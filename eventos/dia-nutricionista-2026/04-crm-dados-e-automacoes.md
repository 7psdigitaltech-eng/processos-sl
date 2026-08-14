# 04 — CRM, dados e automações

## 1. Princípio arquitetural

O CRM deve concentrar a **jornada de relacionamento com a convidada**.

O ERP/Bling permanece como sistema operacional para processos como pedido, estoque, faturamento e contas.

```text
WhatsApp
   ↓
Landing page
   ↓
CRM / Evento
   ├── convite
   ├── interação
   ├── confirmação
   ├── presença
   └── pós-evento
            ↓
      oportunidade/relacionamento
            ↓
          ERP/Bling
      quando houver operação comercial
```

## 2. Entidades conceituais

### Contato / Nutricionista

Cadastro principal da profissional.

Campos existentes no CRM devem ser reaproveitados. O evento não deve criar um cadastro paralelo.

### Evento

Representa a edição do encontro.

Campos mínimos:

- `evento_id`
- `nome`
- `data`
- `status`
- `local`
- `capacidade`

### Convite de evento

Relação entre uma nutricionista e um evento.

Campos sugeridos:

- `evento_convite_id`
- `evento_id`
- `contato_id`
- `token`
- `status`
- `enviado_em`
- `acessado_em`
- `confirmado_em`
- `recusado_em`
- `presenca_em`
- `ultimo_contato_em`
- `origem_convite`

## 3. Status da jornada

O status deve refletir a situação atual, sem perder os timestamps dos eventos anteriores.

```text
CONVITE_PREPARADO
      ↓
CONVITE_ENVIADO
      ↓
ACESSOU
      ↓
┌───────────────┬─────────────────┐
│               │                 │
▼               ▼                 ▼
CONFIRMADA   RECUSADA          PENDENTE
│                                │
▼                                ▼
PRESENÇA                     LEMBRETES
│
▼
PÓS-EVENTO
```

### Observação

`PENDENTE` não é um estado final. É a condição de quem recebeu/visitou o convite e ainda não registrou uma decisão.

## 4. Eventos de sistema

Além do status atual, registrar eventos importantes:

| Evento | Quando ocorre |
|---|---|
| `convite_preparado` | convite pronto para envio |
| `convite_enviado` | mensagem disparada com sucesso |
| `landing_acessada` | convite individual abriu a página |
| `presenca_confirmada` | confirmação registrada |
| `presenca_recusada` | impossibilidade registrada |
| `lembrete_enviado` | lembrete disparado |
| `presenca_registrada` | presença física registrada |
| `pos_evento_enviado` | comunicação pós-evento disparada |

Os eventos servem para auditoria, métricas e automação.

## 5. Automação de WhatsApp

### Fluxo 1 — Convite

Disparar para cada convidada com o link individual.

### Fluxo 2 — Follow-up de não resposta

Critério conceitual:

`convite enviado + prazo definido + sem confirmação/recusa`

A automação envia lembrete sem alterar artificialmente o status para ausência.

### Fluxo 3 — Confirmação

Ao confirmar:

1. atualizar a relação convidada/evento;
2. registrar `presenca_confirmada`;
3. registrar data/hora;
4. cancelar lembretes de confirmação ainda pendentes;
5. enviar mensagem de agradecimento;
6. iniciar jornada pré-evento.

### Fluxo 4 — Recusa

Ao informar que não poderá comparecer:

1. atualizar status para `RECUSADA`;
2. registrar evento de recusa;
3. cancelar lembretes;
4. agradecer;
5. manter o contato disponível para relacionamento futuro.

### Fluxo 5 — Pré-evento

Enviar informações práticas conforme calendário definido.

### Fluxo 6 — Pós-evento

Enviar agradecimento e conteúdo pós-evento para quem compareceu. Para quem não compareceu, usar comunicação diferente e não presumir participação.

## 6. Personalização pós-evento

Depois da presença, a nutricionista pode receber uma próxima ação conforme perfil.

Exemplos:

```text
PRESENÇA
   ↓
PERFIL
   ├── Home Care → relacionamento Home Care
   ├── Hospitalar → soluções hospitalares
   ├── Clínica → soluções clínicas
   └── Outro → relacionamento geral
```

A segmentação deve utilizar dados já existentes no CRM sempre que possível.

## 7. Prevenção de duplicidade

A confirmação de presença deve atualizar a relação entre contato e evento.

Não criar:

- novo contato;
- novo cadastro de nutricionista;
- novo lead apenas para a confirmação.

Caso a profissional ainda não exista no CRM, a criação do contato deve seguir a regra geral de cadastro definida para a Santa Luzia.

## 8. Integrações

Integrações previstas conceitualmente:

- **WhatsApp** — convite e mensagens;
- **Landing page** — captura de interação e confirmação;
- **CRM** — cadastro e jornada;
- **n8n ou motor de automação** — orquestração;
- **Bling/ERP** — somente quando surgir operação comercial/administrativa que pertença ao ERP.

A tecnologia definitiva de cada integração ainda está pendente de decisão.

## 9. Privacidade e governança

Coletar apenas dados necessários para convite, confirmação, logística e relacionamento planejado.

O projeto deve definir antes da implantação:

- finalidade dos dados coletados;
- permissões de acesso;
- prazo de retenção;
- política de exclusão/anonimização, quando aplicável;
- responsáveis pela gestão do dado.
