# 06 — Backlog e pendências

## 1. Decisões já fechadas

- [x] Data: 29/08/2026.
- [x] Início: 19h.
- [x] Local: YBY Condomínio Boutique, Ananindeua/PA.
- [x] Endereço: Travessa Thenry, BR-316, S/N, Ananindeua - PA, 67113-120.
- [x] Capacidade estimada: aproximadamente 60 pessoas.
- [x] Convite individual, sem acompanhante.
- [x] Dress code: social/coquetel.
- [x] Estacionamento próprio.
- [x] WhatsApp de dúvidas: (91) 99294-4871.
- [x] Nome do projeto: Experiência Digital — Dia do Nutricionista 2026.
- [x] Link geral para todas as convidadas.
- [x] Sem token ou URL nominal.
- [x] Confirmação em modal na própria página.
- [x] Confirmação primeiro → enriquecimento depois.
- [x] WhatsApp Business operado manualmente.
- [x] CRM atual da Santa Luzia, no kanban específico de nutricionistas.
- [x] Supabase como camada de dados da experiência.
- [x] Marcas: NUTRO e PRODIET.
- [x] Evento como protagonista; produtos não serão apresentados em formato de venda.

## 2. Prioridade P0 — necessárias antes do desenvolvimento final

- [ ] Definir data limite de confirmação.
- [ ] Fechar sequência definitiva da programação.
- [ ] Definir responsável pelo check-in.
- [ ] Definir como o contato será localizado no CRM pelo WhatsApp informado na confirmação.
- [ ] Definir regra de criação de contato quando a nutricionista ainda não existir no CRM.
- [ ] Definir política de privacidade definitiva.
- [ ] Definir domínio/subdomínio da experiência na VPS.
- [ ] Definir estratégia de backup/monitoramento da página e banco.

## 3. Prioridade P1 — conteúdo e implementação

- [ ] Finalizar copy da landing page.
- [ ] Finalizar identidade visual digital.
- [ ] Preparar imagens do ambiente.
- [ ] Preparar logo oficial Santa Luzia.
- [ ] Preparar logos oficiais NUTRO e PRODIET.
- [ ] Definir produtos/soluções que eventualmente serão destacados.
- [ ] Publicar landing page na VPS.
- [ ] Criar evento no CRM.
- [ ] Criar relação nutricionista/evento.
- [ ] Implementar confirmação/recusa.
- [ ] Implementar prevenção de duplicidade.
- [ ] Implementar registro de presença.
- [ ] Criar indicadores/relatório.
- [ ] Realizar teste ponta a ponta com convidados internos.

## 4. Prioridade P2 — melhoria da experiência

- [ ] Preservar visualmente o estado de confirmação no mesmo navegador.
- [ ] Criar conteúdo pós-evento.
- [ ] Criar galeria/fotos pós-evento.
- [ ] Criar CTA de relacionamento com equipe Santa Luzia.
- [ ] Registrar interações relevantes para futuras ações.
- [ ] Personalizar relacionamento pós-evento por perfil profissional.

## 5. Decisões de produto/negócio

### Individualização do convite

**Decisão:** link geral para todas as convidadas. Não utilizar token ou URL nominal.

### Confirmação

**Decisão:** confirmar/recusar na própria landing page, usando modal e poucos campos.

### Cadastro

**Decisão:** reaproveitar contato existente no CRM e criar apenas a relação com o evento.

### Dados

**Decisão:** confirmação exige somente o necessário. Enriquecimento profissional ocorre depois.

### WhatsApp

**Decisão:** operação manual pelo WhatsApp Business. Não depender de automação de mensagens na primeira versão.

### Comercialização

**Decisão:** não transformar a confirmação em fluxo de venda. A página apresenta Santa Luzia, NUTRO e PRODIET de forma institucional e contextual.

### Pós-evento

**Decisão:** criar jornada específica para participantes e tratamento diferente para convidadas que não compareceram.

## 6. Critério de pronto — MVP

O MVP pode ser considerado pronto quando uma convidada conseguir:

1. receber o convite pelo WhatsApp;
2. abrir o link geral;
3. visualizar os detalhes essenciais;
4. abrir o modal de confirmação;
5. confirmar ou recusar presença;
6. continuar navegando pela experiência;
7. ter a informação gravada no CRM sem duplicidade;
8. ter a presença marcada no evento;
9. entrar na jornada pós-evento adequada.

## 7. Próxima etapa recomendada

Transformar o planejamento em tarefas separadas:

- **Produto/UX** — wireframe e interface da experiência;
- **Copy** — refinamento dos textos e validação de claims;
- **Frontend** — implementação da landing page;
- **Supabase** — tabelas, regras e eventos;
- **CRM** — integração e kanban de nutricionistas;
- **Operação** — lista, WhatsApp, check-in e follow-up;
- **Marketing** — identidade, fotos e ativos de marcas;
- **Dados** — indicadores e relatório.
