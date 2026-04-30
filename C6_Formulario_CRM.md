# FORMULÁRIO CRM — C6 PROPOSTA, NEGOCIAÇÃO E FECHAMENTO

## 1. Objetivo do Formulário

Padronizar o registro da etapa C6 no CRM, garantindo que toda proposta, negociação e fechamento sejam rastreáveis, controlados e conectados à operação.

Este formulário deve apoiar:

- preparação da proposta;
- envio de orçamento;
- controle de validade;
- negociação;
- aprovação de desconto;
- fechamento;
- encaminhamento para pedido/entrega;
- registro de perda;
- criação de recorrência.

---

# 2. Bloco: Identificação da Oportunidade

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Nome do cliente/paciente/instituição | Texto | Sim | Deve vir da oportunidade |
| Tipo de cliente | Lista | Sim | Familiar / Home Care / Hospital / Clínica / Nutricionista / Institucional / Outro |
| Responsável pelo contato | Texto | Sim | Pessoa com quem a equipe fala |
| Responsável pela decisão | Texto | Sim | Quem aprova a compra |
| Responsável pelo pagamento | Texto | Sim | Pessoa ou instituição pagadora |
| Etapa anterior concluída | Lista | Sim | C4 concluída / C5 acionada / Venda direta / Outro |
| Existe objeção ativa? | Sim/Não | Sim | Se sim, conectar com C5 |

---

# 3. Bloco: Preparação da Proposta

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Produto validado | Texto | Sim | Produto que será cotado/vendido |
| Apresentação do produto | Texto | Condicional | Ex.: unidade, caixa, frasco, lata, equipo |
| Quantidade validada | Número | Sim | Quantidade considerada na proposta |
| Quantidade mensal estimada | Número | Condicional | Obrigatório para venda recorrente |
| Tipo de venda | Lista | Sim | Pontual / Recorrente / Institucional / Indefinida |
| Prescrição/documento conferido? | Sim/Não/Não se aplica | Sim | Quando aplicável |
| Estoque/disponibilidade conferido? | Sim/Não/Não se aplica | Sim | Usar quando houver risco de falta |
| Entrega validada? | Sim/Não/Não se aplica | Sim | Confirmar antes de prometer prazo |
| Condição de pagamento prevista | Lista | Sim | Pix / Cartão / Faturado / Boleto / Outro |
| Necessita proposta formal? | Sim/Não | Sim | Sim para institucional ou quando cliente solicitar |
| Observações para proposta | Texto longo | Não | Condições, restrições ou informações relevantes |

---

# 4. Bloco: Envio da Proposta

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Proposta enviada? | Sim/Não | Sim | Gate da C6 |
| Data de envio da proposta | Data | Condicional | Obrigatório se proposta enviada |
| Canal de envio | Lista | Condicional | WhatsApp / E-mail / PDF / Presencial / Outro |
| Tipo de proposta | Lista | Sim | Simples / Recorrente / Institucional |
| Valor unitário | Moeda | Condicional | Quando aplicável |
| Valor total da proposta | Moeda | Sim | Valor total enviado ao cliente |
| Validade da proposta | Data | Sim | Toda proposta deve ter validade |
| Prazo de entrega informado | Texto | Sim | Ex.: imediato, 24h, 48h, sob consulta |
| Condição de pagamento informada | Texto | Sim | Igual ao enviado ao cliente |
| Itens inclusos | Texto longo | Não | Ex.: produto, entrega, acessórios |
| Itens não inclusos | Texto longo | Não | Quando necessário |
| Mensagem/proposta anexada | Upload ou link | Recomendado | Evidência do que foi enviado |

---

# 5. Bloco: Validação de Entendimento

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Cliente confirmou entendimento da proposta? | Sim/Não | Sim | Confirmar se a proposta ficou clara |
| Produto e quantidade confirmados? | Sim/Não | Sim | Evita erro antes do fechamento |
| Prazo de entrega atende? | Sim/Não/Não informado | Sim | |
| Forma de pagamento atende? | Sim/Não/Não informado | Sim | |
| Existe comparação com concorrente? | Sim/Não | Sim | Se sim, detalhar |
| Concorrente informado | Texto | Não | Se cliente mencionar |
| Comparação é equivalente? | Sim/Não/Não identificado | Condicional | Produto, quantidade, entrega e marca iguais? |
| O que falta para fechar? | Texto longo | Sim | Ex.: pagamento, aprovação, desconto, documento |
| Decisor final confirmado? | Sim/Não | Sim | |

---

# 6. Bloco: Negociação

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Houve negociação? | Sim/Não | Sim | |
| Tipo de negociação | Lista | Condicional | Preço / Prazo / Pagamento / Entrega / Volume / Recorrência / Documentação / Outro |
| Motivo da negociação | Texto longo | Condicional | Obrigatório se houve negociação |
| Objeção relacionada | Lista | Não | Preço / Fornecedor / Orçamento / Logística / Decisor / Outro |
| C5 acionada? | Sim/Não | Condicional | Se houve objeção relevante |
| Alternativa ao desconto avaliada? | Sim/Não | Condicional | Ex.: volume, prazo, recorrência |
| Desconto solicitado? | Sim/Não | Sim | |
| Valor ou percentual solicitado | Texto | Condicional | Se cliente pediu desconto |
| Desconto concedido? | Sim/Não | Sim | |
| Valor ou percentual concedido | Texto | Condicional | Se concedido |
| Desconto aprovado por quem? | Texto | Condicional | Obrigatório se desconto concedido |
| Margem mínima preservada? | Sim/Não/Não avaliado | Condicional | Conforme regra interna |
| Condição especial concedida | Texto longo | Não | Ex.: entrega, prazo, parcelamento |
| Validade da condição especial | Data | Condicional | Quando houver condição especial |

---

# 7. Bloco: Fechamento

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Status da C6 | Lista | Sim | Proposta em preparação / Proposta enviada / Validação de entendimento / Em negociação / Aguardando pagamento / Aguardando documento / Pedido fechado / Recorrência programada / Perdida / Desqualificada |
| Pedido fechado? | Sim/Não | Sim | |
| Data de fechamento | Data | Condicional | Obrigatório se pedido fechado |
| Pagamento confirmado? | Sim/Não/Não se aplica | Sim | |
| Forma de pagamento final | Lista | Condicional | Pix / Cartão / Faturado / Boleto / Outro |
| Comprovante anexado? | Sim/Não/Não se aplica | Não | |
| Documento pendente? | Sim/Não | Sim | |
| Qual documento pendente? | Texto | Condicional | Prescrição / NF / Cadastro / Empenho / Autorização / Outro |
| Entrega acionada? | Sim/Não/Não se aplica | Sim | |
| Data prevista de entrega | Data | Condicional | Obrigatório se houver entrega |
| Responsável pelo recebimento | Texto | Condicional | Obrigatório se houver entrega |
| Observações de entrega | Texto longo | Não | Restrições, horários, ponto de referência |
| Pedido registrado internamente? | Sim/Não | Sim | |

---

# 8. Bloco: Recorrência

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Recorrência identificada? | Sim/Não | Sim | |
| Recorrência criada? | Sim/Não | Condicional | Obrigatório se recorrência identificada |
| Frequência de recompra | Lista | Condicional | Semanal / Quinzenal / Mensal / Outro |
| Quantidade por ciclo | Número | Condicional | Quantidade prevista por recompra |
| Data da próxima recompra | Data | Condicional | |
| Responsável pelo acompanhamento | Texto | Condicional | |
| Cliente aceitou lembrete de recompra? | Sim/Não | Não | |

---

# 9. Bloco: Follow-up

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Próximo passo | Texto longo | Sim | Nenhuma C6 pode ficar sem próximo passo |
| Responsável pelo próximo passo | Texto | Sim | |
| Data de follow-up | Data | Sim | |
| Canal de follow-up | Lista | Não | WhatsApp / Ligação / E-mail / Presencial |
| Tentativa de follow-up atual | Número | Não | Ex.: 1, 2, 3 |
| Observação do follow-up | Texto longo | Não | |

---

# 10. Bloco: Perda ou Desqualificação

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Venda perdida? | Sim/Não | Sim | |
| Motivo de perda | Lista | Condicional | Preço / Prazo / Concorrente / Sem orçamento / Sem documento / Logística / Desistência / Sem resposta / Outro |
| Concorrente escolhido | Texto | Não | Se conhecido |
| Valor perdido | Moeda | Não | Ajuda em análise futura |
| Pode retomar futuramente? | Sim/Não | Não | |
| Data de retomada futura | Data | Condicional | Se fizer sentido nutrir |
| Observações da perda | Texto longo | Não | |

---

# 11. Regras de Uso do Formulário

## Regra 1 — Não enviar proposta sem dados mínimos

Antes de enviar proposta, precisam estar preenchidos:

- produto validado;
- quantidade validada;
- responsável pela decisão;
- responsável pelo pagamento;
- condição de entrega;
- condição de pagamento prevista.

---

## Regra 2 — Toda proposta precisa ter validade

O campo **Validade da proposta** é obrigatório para proteger a empresa contra:

- alteração de preço;
- falta de estoque;
- mudança de condição comercial;
- uso de orçamento antigo.

---

## Regra 3 — Toda proposta precisa de follow-up

Nenhuma proposta deve ficar sem:

- próximo passo;
- responsável;
- data de follow-up.

---

## Regra 4 — Desconto exige registro

Se houver desconto, registrar:

- motivo;
- valor ou percentual;
- responsável pela aprovação;
- validade da condição;
- se a margem mínima foi preservada.

---

## Regra 5 — WhatsApp é canal, CRM é registro

A proposta pode ser enviada por WhatsApp, mas o CRM deve guardar o histórico oficial da C6.

---

## Regra 6 — Promessa operacional precisa ser validada

Não prometer prazo, entrega, estoque, reserva ou condição especial sem validação interna.

---

## Regra 7 — Venda recorrente gera agenda

Se houver recorrência, deve ser criada uma data de recompra e um responsável pelo acompanhamento.

---

# 12. Versão Mínima para Implantação Inicial

Caso o CRM precise começar de forma mais simples, usar inicialmente apenas os campos abaixo:

| Campo | Tipo | Obrigatório |
|------|------|------------|
| Produto validado | Texto | Sim |
| Quantidade validada | Número | Sim |
| Proposta enviada | Sim/Não | Sim |
| Data de envio | Data | Condicional |
| Valor total | Moeda | Sim |
| Validade da proposta | Data | Sim |
| Status da C6 | Lista | Sim |
| Houve negociação | Sim/Não | Sim |
| Houve desconto | Sim/Não | Sim |
| Próximo passo | Texto | Sim |
| Responsável | Texto | Sim |
| Data de follow-up | Data | Sim |
| Pedido fechado | Sim/Não | Sim |
| Recorrência criada | Sim/Não | Condicional |
| Motivo de perda | Lista | Condicional |

---

# 13. Resultado Esperado

Com este formulário, a Santa Luzia passa a ter uma C6 mais controlada, reduzindo:

- propostas incompletas;
- descontos sem critério;
- perdas por falta de follow-up;
- promessas operacionais incorretas;
- perda de histórico no WhatsApp;
- falta de controle sobre recorrência;
- ausência de motivo de perda.

O formulário também melhora:

- conversão de proposta em pedido;
- preservação de margem;
- rastreabilidade comercial;
- organização da entrega;
- previsibilidade de receita;
- aprendizado sobre negociações perdidas.
