# PROPOSTA — ESTRUTURA COMPLETA DA ÁREA COMERCIAL
**Status:** ✅ 100% VALIDADO — pronto para documentação (13/04/2026)
**Data:** 13 de abril de 2026
**Insumos:** Atas Reunião 04 + 05 + Pesquisa de Boas Práticas
**Cenário:** Misto A + B — processos existem informalmente, com gaps críticos

---

## ✅ DECISÕES VALIDADAS POR EDUARDO (13/04/2026)

| Ponto | Decisão tomada |
|---|---|
| Ferramenta de pipeline | **Notion** no início → **CRM próprio com IA** após alinhamento dos processos |
| Divisão Maria × Júlia | **Maria:** C1, C2, C3 (captação, qualificação, prospecção) + apoio em visitas técnicas / **Júlia:** C4 (visita técnica) como responsável principal |
| Autonomia para negociação | **Fechamento é Eyder** — vendedoras não têm autonomia para negociar condições finais |
| Canal WhatsApp | **Número da empresa** (não pessoal) |
| C3 — Cadência | Inclui **ligação** além de WhatsApp e email — 3 canais simultâneos |

---

## LÓGICA DA ESTRUTURA

A área comercial da Santa Luzia precisa funcionar em **dois grandes blocos**:

1. **Bloco de Aquisição** — trazer novos clientes (do lead ao primeiro pedido)
2. **Bloco de Retenção** — manter e expandir clientes ativos (da recorrência ao crescimento de carteira)

Hoje a empresa opera quase inteiramente no bloco 1, de forma informal. O bloco 2 existe na prática (os clientes continuam comprando), mas sem processo definido — funciona pelo relacionamento pessoal do Eyder.

A proposta abaixo organiza os dois blocos em **10 processos**, sendo 6 prioritários (escopo contratual) e 4 de suporte (aditivo ou segunda fase).

---

## VISÃO GERAL — OS 10 PROCESSOS PROPOSTOS

### 🟦 BLOCO 1 — AQUISIÇÃO DE NOVOS CLIENTES

| # | Processo | Responsável | Situação atual | Prioridade |
|---|---|---|---|---|
| C1 | Geração e captação de leads | Maria | Existe — sem critério | 🔴 Alta |
| C2 | Triagem e qualificação de leads | Maria + Eyder | Existe — empírico | 🔴 Alta |
| C3 | Cadência de prospecção multicanal | Maria + Júlia | Não existe | 🔴 Alta |
| C4 | Visita técnica comercial | Júlia + Eyder | Existe — sem roteiro | 🔴 Alta |
| C5 | Gestão de objeções | Júlia + Eyder | Não existe | 🟡 Média |
| C6 | Negociação e fechamento | Eyder | Existe — centralizado | 🟡 Média |

### 🟩 BLOCO 2 — RETENÇÃO E CRESCIMENTO DE CARTEIRA

| # | Processo | Responsável | Situação atual | Prioridade |
|---|---|---|---|---|
| C7 | Gestão de carteira e recorrência | Maria + Júlia | Existe — no feeling | 🔴 Alta |
| C8 | Handoff comercial → operacional | Eyder → Pablo | Não existe | 🟡 Média |
| C9 | Re-engajamento de leads frios | Maria | Não existe | 🟡 Média |

### 🟧 SUPORTE — GESTÃO DO TIME

| # | Processo | Responsável | Situação atual | Prioridade |
|---|---|---|---|---|
| C10 | Métricas e acompanhamento da equipe | Eyder | Não existe | 🟡 Média |

---

## FLUXO INTEGRADO — COMO OS PROCESSOS SE CONECTAM

```
LEAD IDENTIFICADO
       │
       ▼
[C1] GERAÇÃO DE LEADS ──────────────────────────────────────────────┐
  (Maria captura via IA, site OS, indicação)                        │
       │                                                            │
       ▼                                                            │
[C2] TRIAGEM E QUALIFICAÇÃO                                         │
  (BANT simplificado: orçamento, autoridade, necessidade, timing)   │
       │                                                            │
       ├── Lead NÃO qualificado ──────────────────────────────► [C9] RE-ENGAJAMENTO
       │                                                         (90 dias depois)
       ▼
[C3] CADÊNCIA DE PROSPECÇÃO MULTICANAL
  (10 dias: WhatsApp D0 + Email D1 + WA D3 + Email D6 + WA D10)
       │
       ├── Sem resposta após 3 ciclos ──────────────────────────► [C9] RE-ENGAJAMENTO
       │
       ▼
[C4] VISITA TÉCNICA COMERCIAL
  (reunião com nutricionista + comprador — roteiro padronizado)
       │
       ├── Objeção identificada ──────────────────────────────► [C5] GESTÃO DE OBJEÇÕES
       │                                                         (resposta, contorno, piloto)
       ▼
[C6] NEGOCIAÇÃO E FECHAMENTO
  (proposta de preço, condições, documentação)
       │
       ▼
[C8] HANDOFF COMERCIAL → OPERACIONAL
  (briefing de novo cliente, primeiro pedido)
       │
       ▼
[C7] GESTÃO DE CARTEIRA E RECORRÊNCIA
  (ciclo mensal: pedidos, visitas, expansão)
       │
       └── Ativo ──────────────────────────────────────────────► Continua em C7
       
[C10] MÉTRICAS E ACOMPANHAMENTO (roda em paralelo, toda semana)
```

---

## DETALHAMENTO DE CADA PROCESSO

---

### C1 — GERAÇÃO E CAPTAÇÃO DE LEADS

**Cenário:** B (existe, mas sem critério documentado)
**Responsável sugerido:** Maria
**Gatilho:** Início de semana (rotina) ou identificação de nova OS/hospital

**Fluxo proposto:**
1. Acessar base de OS por estado (site das OS ou lista existente no Notion)
2. Identificar hospitais administrados pela OS que ainda não são clientes
3. Pesquisar contatos: nutricionista responsável + comprador/gestor
4. Registrar no pipeline (CRM/planilha): nome, instituição, contato, tipo, estado
5. Classificar prioridade: OS > Hospital Particular > Home Care; dentro do tipo: maior hospital primeiro

**Critério de conclusão:** Lead registrado no pipeline com campos mínimos preenchidos (nome, instituição, contato, tipo)

**Meta sugerida:** 8-10 novos leads por semana (Maria)

**Pontos de decisão do dono:**
- ⚠️ Ferramenta: manter Notion atual ou migrar para CRM (Bigin/Agendor)?
- ⚠️ Maria faz isso sozinha ou Eyder revisa semanalmente?

---

### C2 — TRIAGEM E QUALIFICAÇÃO DE LEADS

**Cenário:** B (existe de forma empírica, sem critério)
**Responsável sugerido:** Maria (executa) + Eyder (valida dúvidas)
**Gatilho:** Lead captado em C1 precisa ser avaliado antes de entrar na prospecção ativa

**Critério BANT simplificado para a Santa Luzia:**

| Pergunta | Como descobrir | Resposta que qualifica |
|---|---|---|
| **Budget (Orçamento):** O hospital compra dieta enteral regularmente? | Site, CNES, porte do hospital | Sim — tem histórico de compra |
| **Authority (Autoridade):** Conseguimos falar com nutricionista ou comprador? | Pesquisa + primeiro contato | Tem contato identificado |
| **Need (Necessidade):** Eles têm problema com fornecedor atual? | Primeiro contato / visita | Abertura para conversa |
| **Timing (Momento):** Quando é o próximo ciclo de compra? | Ligação inicial | Tem janela em até 90 dias |

**Classificação de leads:**
- 🔴 **Quente:** Respondeu + passou BANT → vai direto para C3
- 🟡 **Morno:** Respondeu parcialmente → entra em C3 com abordagem cuidadosa
- 🔵 **Frio:** Não respondeu ou não passou BANT → arquivo + C9 (reativação em 90 dias)

**Critério de conclusão:** Todo lead com status definido (quente/morno/frio) no pipeline

**Pontos de decisão do dono:**
- ⚠️ Quem faz a qualificação de leads de OS (maior complexidade) — Maria ou Eyder?

---

### C3 — CADÊNCIA DE PROSPECÇÃO MULTICANAL

**Cenário:** A (não existe — cada vendedor faz do seu jeito)
**Responsável sugerido:** Maria e Júlia (para Belém); Eyder (para outras cidades/OS remotas)
**Gatilho:** Lead qualificado (quente ou morno) em C2

**Cadência proposta (12 dias — 3 canais: WhatsApp + Email + Ligação):**

| Dia | Canal | Ação | Modelo / Orientação |
|---|---|---|---|
| **D0** | WhatsApp | Primeiro contato — curto + pergunta | "Olá [Nome], sou [Nome] da Santa Luzia, distribuidora de dieta enteral em Belém. Vi que [hospital X] atende pacientes que usam nutrição enteral. Têm 5 minutos essa semana pra conversar?" |
| **D1** | Email | Apresentação + 3 diferenciais + CTA | Portfólio + entrega em 2 dias + referência de hospital similar + pedido de reunião |
| **D3** | Ligação | Primeiro contato por voz | Citar o WhatsApp e o email enviados. Se não atender: deixar recado curto + WhatsApp logo após. Se atender: diagnóstico rápido (2-3 perguntas BANT) |
| **D5** | WhatsApp | Follow-up pós-ligação | "Olá [Nome], tentei te ligar. Vi que [hospital] usa dieta enteral. Posso mandar mais info por aqui?" |
| **D7** | Email | Case de hospital similar + prova social | "Veja como o [Hospital X] em Belém economizou com nossa distribuição..." |
| **D10** | Ligação | Segunda tentativa por voz | Citar o case enviado. Foco: agendar visita técnica de 30 min sem compromisso |
| **D12** | WhatsApp | Encerramento educado | "Tentei contato algumas vezes. Se não for o momento, tudo bem — fica a porta aberta. Qualquer mudança, é só chamar." |

**Regras de ouro:**
- Usar sempre o **número da empresa** (não número pessoal)
- Nunca ligar sem antes ter enviado WhatsApp ou email no mesmo dia ou anterior
- Se atender na ligação e demonstrar interesse → pular os passos restantes e agendar visita diretamente
- Registrar cada tentativa no pipeline: data + canal + resultado (atendeu / não atendeu / respondeu / ignorou)
- Nunca mencionar concorrente negativamente

**Regras de ouro:**
- Nunca ligar sem antes ter enviado WhatsApp ou email
- Nunca mencionar concorrente negativamente
- Se o decisor mudar, reiniciar cadência com novo contato
- Registrar cada tentativa no pipeline (data + canal + resultado)

**Critério de conclusão:** Lead respondeu (positivo → vai para C4) OU cadência encerrada sem resposta (→ C9)

**Pontos de decisão do dono:**
- ⚠️ Júlia faz prospecção ou só visitas? (definir divisão de papel entre Maria e Júlia)
- ⚠️ Usar número pessoal ou número da empresa no WhatsApp?

---

### C4 — VISITA TÉCNICA COMERCIAL

**Cenário:** B (existe, mas sem roteiro padronizado)
**Responsável sugerido:** Júlia (visitas em Belém) + Eyder (visitas estratégicas ou outras cidades)
**Gatilho:** Lead respondeu positivamente em C3 e aceitou reunião

**Roteiro de visita (estrutura em 5 etapas):**

**PRÉ-VISITA (D-1 antes da visita):**
- Confirmar reunião por WhatsApp na véspera
- Levar: portfólio físico + amostras + folder de referências de hospitais atendidos
- Pesquisar: qual fornecedor atual, porte do hospital, nome do nutricionista e comprador

**NA VISITA — Com a Nutricionista:**
1. Abertura: "Como está funcionando a dieta enteral que vocês usam hoje?"
2. Escuta ativa — deixar ela falar (não interromper)
3. Diagnóstico: "O que é mais importante pra você: disponibilidade, qualidade, custo ou atendimento?"
4. Apresentação: apresentar produto focado no que ela priorizou
5. Proposta de teste: "Posso deixar amostras para teste clínico? Sem compromisso."

**NA VISITA — Com o Comprador/Gestor:**
1. Abertura: "Como funciona o processo de compra de vocês?"
2. Ciclo: "Quando é feito o pedido mensal?"
3. Fornecedores: "Quantos fornecedores participam das cotações?"
4. Apresentação: focar em prazo de entrega + preço + condições

**REGISTRAR após a visita (no mesmo dia):**
- Nome e contato do nutricionista e comprador
- Principal preocupação de cada um
- Próximo passo combinado (ex: aguardar aprovação de amostras, data de cotação)
- Nível de interesse: alto / médio / baixo

**PÓS-VISITA (até 24h depois):**
- WhatsApp de agradecimento para quem visitou
- Email com portfólio + proposta se combinado na visita

**Critério de conclusão:** Visita realizada, informações registradas, próximo passo definido

**Pontos de decisão do dono:**
- ⚠️ Júlia vai sozinha ou sempre acompanha Eyder nas primeiras visitas?
- ⚠️ Onde registrar as informações da visita — WhatsApp grupo, planilha ou CRM?

---

### C5 — GESTÃO DE OBJEÇÕES

**Cenário:** A (não existe — cada um improvisa na hora)
**Responsável sugerido:** Júlia + Eyder (para casos mais complexos)
**Gatilho:** Objeção identificada em C4 (visita) ou C3 (prospecção)

**As 3 objeções mais comuns e como responder:**

**OBJEÇÃO 1: "Já temos fornecedor, não queremos trocar"**
- Não atacar o fornecedor atual
- Resposta: _"Entendo. O que ouço de outros hospitais é que muitas vezes o fornecedor atual é bom, mas tem espaço para otimizar. Posso fazer um teste com 3 produtos por 30 dias? Se não funcionar melhor, sem custo e sem compromisso."_
- Próximo passo: proposta de piloto com prazo definido

**OBJEÇÃO 2: "Preço muito alto"**
- Questionar antes de defender: _"Comparado a quem? É só o preço ou tem alguma outra preocupação?"_
- Reframear para custo total: _"O nosso preço é X% acima, mas entregamos em 2 dias — você nunca fica sem produto. Quanto custa ficar sem dieta enteral para um paciente 24h?"_
- Se o preço for real: oferecer volume mínimo ou condição especial no primeiro pedido

**OBJEÇÃO 3: "Não temos orçamento agora"**
- Descobrir: _"Quando é a revisão do orçamento de vocês?"_
- Agendar contato 15-30 dias antes dessa data
- Enquanto isso: manter aquecimento com artigo ou publicação técnica

**Regra de ouro:** Toda objeção registrada no pipeline com a resposta usada e o resultado — isso vira base de treinamento para a equipe.

**Critério de conclusão:** Objeção respondida, próximo passo definido (piloto, revisão de preço, agendamento futuro ou lead arquivado)

**Pontos de decisão do dono:**
- ⚠️ Júlia tem autonomia para oferecer piloto de 30 dias sem consultar Eyder?
- ⚠️ Qual é o desconto máximo que Júlia/Maria podem dar sem aprovação?

---

### C6 — NEGOCIAÇÃO E FECHAMENTO

**Cenário:** B (existe, mas centralizado em Eyder)
**Responsável sugerido:** Eyder (decisão final) + Júlia (preparação da proposta)
**Gatilho:** Nutricionista deu aval técnico / Comprador pediu cotação formal

**Fluxo proposto:**
1. Júlia ou Maria prepara proposta: produtos + quantidades + preço (tabela vigente) + prazo de entrega
2. Eyder revisa e aprova proposta antes de enviar
3. Enviar por email com cópia WhatsApp para confirmar recebimento
4. Aguardar resposta no prazo combinado (máximo 5 dias úteis)
5. Se aprovado: confirmar data do primeiro pedido + passar para C8 (Handoff)
6. Se não aprovado: identificar motivo → C5 (objeção) ou arquivar

**Critério de conclusão:** Proposta enviada + resposta recebida (positiva ou negativa com motivo registrado)

**Pontos de decisão do dono:**
- ⚠️ Júlia pode enviar proposta sem revisão de Eyder para clientes menores (ticket < R$5k)?
- ⚠️ Qual é o prazo máximo de validade de uma proposta?

---

### C7 — GESTÃO DE CARTEIRA E RECORRÊNCIA

**Cenário:** C (existe no feeling, sem processo)
**Responsável sugerido:** Maria (acompanhamento) + Júlia (visitas) + Eyder (gestão)
**Gatilho:** Cliente fez primeiro pedido e entrou na base ativa

**Ciclo mensal proposto:**

| Momento | Ação | Quem | Como |
|---|---|---|---|
| Início do mês (dia 1-5) | Verificar clientes que ainda não pediram | Maria | Checar pipeline / CRM |
| Dia 5-10 | Antecipar ciclo das OS (pedem dia 10-12 via Bionex) | Maria | WhatsApp com lembrete de cotação |
| Dia 10-15 | Visita de relacionamento mensal | Júlia | Visita presencial + publicação técnica como pretexto |
| Dia 20 | Revisão de clientes sem pedido no mês | Maria + Eyder | Reunião 15 min |
| Último dia do mês | Relatório de carteira (quem comprou, quanto, variação) | Maria | Planilha simples |

**Estratégia de crescimento de carteira:**
- Trazer nova publicação científica ou novidade de produto a cada visita (não ir só para "vender")
- Identificar novos produtos que o cliente poderia usar (substituição ou complemento)
- Mapear outras unidades da mesma OS para expansão

**Critério de conclusão:** Relatório mensal de carteira preenchido

**Pontos de decisão do dono:**
- ⚠️ Maria faz só o acompanhamento por WhatsApp ou também visitas?
- ⚠️ Qual é a frequência mínima de visita por tipo de cliente: OS vs Particular vs Home Care?

---

### C8 — HANDOFF COMERCIAL → OPERACIONAL

**Cenário:** A (não existe — passa verbalmente ou pelo WhatsApp informal)
**Responsável sugerido:** Júlia/Maria (preenche briefing) → Pablo (executa entrega)
**Gatilho:** Negociação fechada — primeiro pedido confirmado

**Checklist obrigatório antes de passar para operação:**

```
BRIEFING DE NOVO CLIENTE

[ ] Nome da instituição
[ ] CNPJ + endereço completo
[ ] Telefone de contato para entrega
[ ] Nome do responsável pelo recebimento
[ ] WhatsApp para comunicação de entrega
[ ] Produtos pedidos + quantidades
[ ] Data de entrega comprometida
[ ] Condições de pagamento (prazo + forma)
[ ] Horário de recebimento preferencial
[ ] Acesso especial (portaria, credencial, etc.)
[ ] Observações especiais (refrigeração, fracionamento)
```

**Pós-entrega (responsabilidade do vendedor):**
- D+1: WhatsApp "Chegou tudo certo?"
- D+7: WhatsApp/ligação rápida "Está tudo funcionando bem?"
- D+30: Cotação para próximo ciclo

**Critério de conclusão:** Checklist preenchido + entrega confirmada pelo cliente

**Pontos de decisão do dono:**
- ⚠️ O briefing vai por WhatsApp grupo ou por formulário/planilha?
- ⚠️ Quem é o responsável pelo follow-up pós-entrega: o vendedor ou Eyder?

---

### C9 — RE-ENGAJAMENTO DE LEADS FRIOS

**Cenário:** A (não existe — leads frios são abandonados)
**Responsável sugerido:** Maria
**Gatilho:** Lead ficou 90 dias sem avanço OU disse "não" há 60+ dias

**Cadência de reativação (45 dias):**

| Dia | Canal | Mensagem |
|---|---|---|
| D0 | WhatsApp | "Olá [Nome], atualização no nosso portfólio — novas marcas e condições. 5 min para conversar?" |
| D3 | Email | Case de hospital similar em Belém com resultado prático |
| D7 | WhatsApp | "Posso fazer um diagnóstico rápido (15 min) para ver se faz sentido pra vocês?" |
| D14 | Email | Condição especial com prazo (ex: "Promoção de portfólio até dia X") |
| D30 | WhatsApp | Encerramento: "Respeito a decisão. Fica a porta aberta — qualquer mudança me chame." |

**Critério de conclusão:** Lead respondeu (→ volta para C2) ou cadência encerrada (→ arquivo final)

**Pontos de decisão do dono:**
- ⚠️ Qual é o período máximo de arquivo antes de considerar o lead definitivamente fora?

---

### C10 — MÉTRICAS E ACOMPANHAMENTO DA EQUIPE

**Cenário:** A (não existe — acompanhamento é por WhatsApp e feeling)
**Responsável sugerido:** Eyder (lidera) + Maria (alimenta dados)
**Gatilho:** Segunda-feira (semanal) e última sexta do mês (mensal)

**Rotina semanal (15 min, toda segunda):**
1. Quantos leads novos Maria captou? (meta: 8-10)
2. Quantas tentativas de contato foram feitas? (meta: 20+ por semana)
3. Quantas propostas foram enviadas?
4. Qual é o lead mais quente agora? Qual é o próximo passo?
5. Alguém precisa de apoio ou desbloqueio?

**Rotina mensal (30-45 min, última sexta):**
1. Faturamento do mês vs. meta
2. Novos clientes conquistados
3. Clientes que não pediram (risco de perda)
4. Leads para reativar (entrada em C9)
5. Taxa de conversão: leads → vendas

**Dashboard mínimo (Google Sheets):**
- Coluna A: Nome do lead/cliente
- Coluna B: Tipo (OS / Particular / Home Care)
- Coluna C: Status no pipeline
- Coluna D: Última ação + data
- Coluna E: Próximo passo + data
- Coluna F: Responsável (Maria / Júlia / Eyder)

**Pontos de decisão do dono:**
- ⚠️ Eyder assume essa reunião semanal ou delega para Eduardo (assessor)?
- ⚠️ Maria preenche a planilha diariamente ou uma vez por semana?

---

## RESUMO EXECUTIVO — DECISÕES

### ✅ Decisões já tomadas
1. **Ferramenta de pipeline:** Notion no início → **CRM próprio com IA** após processos alinhados
2. **Divisão Maria × Júlia:** Maria = C1/C2/C3 + apoio em visitas / Júlia = C4 como responsável principal
3. **Autonomia para negociação:** Fechamento é **Eyder** — vendedoras não negociam condições finais
4. **Canal WhatsApp:** **Número da empresa**
5. **C3 Cadência:** Inclui **3 canais** — WhatsApp + Email + Ligação (12 dias, 7 toques)

### ✅ Decisões adicionais já validadas
6. **Piloto de 30 dias:** **Precisa de aprovação de Eyder** — Júlia não tem autonomia para oferecer sem consultar
7. **Briefing de handoff (C8):** **Separado do Notion** — pode ser integrado aos processos da área operacional depois
8. **Frequência de visita por tipo:** **Hospitais + OS = mínimo 1x/mês** / **Home Care = não define agora** (para segunda fase)
9. **Período de arquivo:** **1 ano** — depois de 1 ano sem resposta, lead é descartado definitivamente
10. **Visão de CRM próprio:** **Quando processos estiverem estruturados e rodando sem erros** — timing de integrações de IA definida depois / Orçamento: a definir depois

---

## PRIORIZAÇÃO SUGERIDA PARA IMPLEMENTAR

### Fase 1 (agora — próximas 2 semanas)
✅ C2 — Qualificação com BANT (baixo esforço, alto impacto imediato)
✅ C3 — Cadência de prospecção (cria rotina para Maria e Júlia)
✅ C8 — Handoff checklist (resolve perda de informação hoje)
✅ C10 — Rotina semanal de 15 min (cria visibilidade imediata)

### Fase 2 (semanas 3-4)
🔜 C4 — Roteiro de visita técnica (aumenta conversão)
🔜 C5 — Gestão de objeções (script + treinamento)
🔜 C7 — Gestão de carteira (ciclo mensal estruturado)

### Fase 3 (mês 2)
🔜 C1 — Captação de leads com ICP definido (escalar volume)
🔜 C6 — Negociação e fechamento (formalizar proposta comercial)
🔜 C9 — Re-engajamento (quando tiver base de leads frios acumulada)

---

## ESCOPO × ADITIVO

**Dentro do contrato (até 6 processos):**
C1, C2, C3, C4, C7, C8 → Os 6 mais críticos para o ciclo completo

**Fora do contrato (aditivo sugerido):**
C5 (Objeções), C6 (Negociação), C9 (Reativação), C10 (Métricas) → 4 processos adicionais

**Recomendação:** Validar com Eyder e propor aditivo de 4 processos ao final do contrato atual.

---

*Proposta elaborada pelo Agente Desenhista de Processo — Projeto Santa Luzia*
*Insumos: Atas Reuniões 04 e 05 + Pesquisa de Boas Práticas (13/04/2026)*
*Status: AGUARDANDO VALIDAÇÃO DE EDUARDO E EYDER*
