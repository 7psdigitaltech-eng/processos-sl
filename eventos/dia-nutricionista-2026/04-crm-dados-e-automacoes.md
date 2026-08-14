# 04 — CRM, dados e automações

## 1. Princípio arquitetural

O CRM deve concentrar a **jornada de relacionamento com a convidada**.

O ERP/Bling permanece como sistema operacional para processos como pedido, estoque, faturamento e contas.

```text
WhatsApp Business — operação manual
   ↓
Experiência Digital / Landing page
   ↓
CRM / Evento
   ├── convite
   ├── confirmação
   ├── recusa
   ├── presença
   └── pós-evento
            ↓
      oportunidade/relacionamento
            ↓
          ERP/Bling
      quando houver operação comercial
```

## 2. Regra de identificação

O projeto utiliza **um link geral**, sem token e sem URL nominal.

Portanto:

- acesso à página = interação anônima/agregada;
- confirmação = momento em que a convidada informa identidade;
- CRM = responsável por localizar o contato existente e associá-lo ao evento.

O sistema não deve tentar adivinhar quem acessou a página.

## 3. Entidades conceituais

### Contato / Nutricionista

Cadastro principal da profissional.

Os campos existentes no CRM devem ser reaproveitados.

O evento não deve criar cadastro paralelo.

### Evento

Representa a edição do encontro.

Campos mínimos:

- `evento_id`
- `nome`
- `data`
- `status`
- `local`
- `capacidade`

### Participação / convite

Relação entre uma nutricionista e um evento.

Campos sugeridos:

- `evento_convite_id`
- `evento_id`
- `contato_id`
- `status`
- `enviado_em`
- `confirmado_em`
- `recusado_em`
- `presenca_em`
- `ultimo_contato_em`
- `origem_convite`
- `observacoes`

**Não utilizar `token` como campo obrigatório do evento**, pois o link geral foi escolhido para esta ação.

## 4. Status da jornada

O status atual deve refletir a situação da convidada sem apagar os timestamps dos eventos anteriores.

```text
CONVITE_PREPARADO
      ↓
CONVITE_ENVIADO
      ↓
┌───────────────┬─────────────────┐
│               │                 │
▼               ▼                 ▼
CONFIRMADA   RECUSADA          PENDENTE
│
▼
PRESENÇA
│
▼
PÓS-EVENTO
```

`PENDENTE` não é um estado final.

## 5. Eventos de sistema

Registrar, quando aplicável:

| Evento | Quando ocorre |
|---|---|
| `convite_preparado` | convite pronto para envio |
| `convite_enviado` | mensagem enviada manualmente e registrada pela equipe |
| `landing_acessada` | página acessada; métrica agregada, sem atribuição individual |
| `presenca_confirmada` | confirmação registrada |
| `presenca_recusada` | impossibilidade registrada |
| `contato_identificado` | dados da confirmação associados a contato do CRM |
| `lembrete_realizado` | equipe realizou follow-up manual |
| `presenca_registrada` | presença física registrada |
| `pos_evento_realizado` | comunicação pós-evento registrada |

Os eventos servem para auditoria, métricas e organização operacional.

## 6. WhatsApp — operação manual

Não haverá automação de mensagens de WhatsApp na primeira versão.

O WhatsApp Business da Santa Luzia será utilizado pela equipe para:

- convite;
- lembrete de pendentes;
- confirmação/agradecimento;
- informações logísticas;
- comunicação do dia do evento;
- pós-evento.

O CRM deve ajudar a equipe a saber **quem precisa de contato**, mas não deve disparar automaticamente essas mensagens.

## 7. Fluxo de confirmação

Ao receber o formulário:

1. validar nome e WhatsApp;
2. localizar contato existente no CRM;
3. se encontrado, reutilizar o contato;
4. associar contato ao evento;
5. registrar confirmação ou recusa;
6. registrar data/hora;
7. impedir duplicidade de relação contato/evento;
8. apresentar feedback na própria página.

### Se o contato não existir

Seguir a regra geral de cadastro da Santa Luzia, evitando criar um cadastro paralelo específico para o evento.

## 8. Enriquecimento posterior

A confirmação não deve coletar perfil profissional detalhado.

Após a confirmação, a equipe poderá complementar:

- atuação Home Care;
- hospitalar;
- clínica;
- consultório;
- especialidades/interesses;
- relacionamento prévio;
- potencial de parceria.

Sempre que possível, aproveitar dados já existentes no CRM.

## 9. Presença

A presença física deve atualizar a mesma relação contato/evento.

Não criar:

- novo contato;
- novo lead apenas para check-in;
- novo cadastro de nutricionista.

## 10. Integrações

### Previstas

- **Landing page ↔ Supabase** — confirmação, estados e eventos;
- **Supabase ↔ CRM** — associação com contato e status;
- **WhatsApp Business** — operação manual, fora de automação;
- **Bling/ERP** — somente quando surgir operação comercial/administrativa pertencente ao ERP.

### Automação

A primeira versão não depende de n8n para WhatsApp.

Se houver automação futura, ela deve ser adicionada sem alterar a regra central do projeto.

## 11. Prevenção de duplicidade

A relação entre contato e evento deve possuir regra de unicidade conceitual:

`contato_id + evento_id = uma participação`

Uma segunda confirmação deve atualizar o registro existente, e não criar outra participação.

## 12. Privacidade e governança

A página deve informar de forma simples que os dados coletados são utilizados para:

- confirmar presença;
- organizar o evento;
- registrar participação;
- realizar o relacionamento planejado pela Santa Luzia.

Definir antes da implantação:

- finalidade dos dados;
- permissões de acesso;
- prazo de retenção;
- política de exclusão/anonimização, quando aplicável;
- responsáveis pela gestão.
