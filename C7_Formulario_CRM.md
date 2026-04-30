# FORMULÁRIO CRM — C7 EXECUÇÃO DO PEDIDO, SEPARAÇÃO, ENTREGA E CONFIRMAÇÃO

## 1. Objetivo do Formulário

Padronizar o registro da etapa C7 no CRM, garantindo que todo pedido fechado seja executado com controle, rastreabilidade e confirmação.

Este formulário deve apoiar:

- recebimento e validação do pedido;
- separação correta dos produtos;
- conferência antes da saída;
- organização da entrega;
- comprovação de recebimento;
- registro de ocorrências;
- atualização operacional;
- criação de recorrência quando aplicável.

---

# 2. Bloco: Identificação do Pedido

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Pedido recebido? | Sim/Não | Sim | Gate inicial da C7 |
| Data do pedido | Data | Sim | Data em que o pedido entrou para execução |
| Origem do pedido | Lista | Sim | C6 / Venda direta / Recorrência / Outro |
| Nome do cliente/paciente/instituição | Texto | Sim | Deve vir da oportunidade |
| Tipo de cliente | Lista | Sim | Familiar / Home Care / Hospital / Clínica / Nutricionista / Institucional / Outro |
| Responsável pelo contato | Texto | Sim | Pessoa de contato principal |
| Responsável pelo recebimento | Texto | Sim | Quem receberá o pedido |
| Telefone do recebedor | Texto | Sim | Contato para entrega |
| Observações vindas da C6 | Texto longo | Não | Condições negociadas, urgência, restrições |

---

# 3. Bloco: Validação do Pedido

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Produto validado | Texto | Sim | Produto vendido/confirmado |
| Apresentação do produto | Texto | Condicional | Ex.: unidade, caixa, lata, frasco, equipo |
| Quantidade vendida | Número | Sim | Quantidade registrada na venda |
| Valor do pedido | Moeda | Sim | Valor total da venda |
| Pagamento confirmado? | Sim/Não/Não se aplica | Sim | Conforme regra interna |
| Condição de pagamento | Lista | Sim | Pix / Cartão / Faturado / Boleto / Outro |
| Documento pendente? | Sim/Não | Sim | Ex.: prescrição, NF, cadastro |
| Qual documento pendente? | Texto | Condicional | Obrigatório se houver documento pendente |
| Pedido completo para execução? | Sim/Não | Sim | Se não, retornar para C6 |
| Prioridade do pedido | Lista | Não | Normal / Urgente / Programado |
| Venda recorrente? | Sim/Não | Sim | Identificar necessidade de recompra |

---

# 4. Bloco: Endereço e Entrega

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Tipo de entrega | Lista | Sim | Entrega própria / Retirada / Motoboy / Transportadora / Outro |
| Endereço confirmado? | Sim/Não | Sim | Não entregar sem endereço validado |
| Endereço completo | Texto longo | Condicional | Obrigatório para entrega |
| Bairro/Cidade | Texto | Condicional | Obrigatório para entrega |
| Ponto de referência | Texto | Não | Ajuda na logística |
| Restrição de acesso | Sim/Não | Não | Condomínio, portaria, horário, escada etc. |
| Descrição da restrição | Texto longo | Condicional | Se houver restrição |
| Janela de entrega | Texto | Não | Ex.: manhã, tarde, até 18h |
| Data prevista de entrega | Data | Sim | |
| Horário previsto | Texto | Não | |
| Cliente precisa ser avisado antes? | Sim/Não | Não | |
| Observações de entrega | Texto longo | Não | |

---

# 5. Bloco: Separação do Pedido

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Produto separado? | Sim/Não | Sim | |
| Responsável pela separação | Texto | Sim | |
| Data/hora da separação | Data/Hora | Sim | |
| Produto correto separado? | Sim/Não | Sim | |
| Apresentação correta? | Sim/Não/Não se aplica | Sim | |
| Quantidade correta separada? | Sim/Não | Sim | |
| Validade conferida? | Sim/Não/Não se aplica | Sim | |
| Data de validade | Data | Condicional | Quando aplicável |
| Lote conferido? | Sim/Não/Não se aplica | Sim | |
| Número do lote | Texto | Condicional | Obrigatório para produtos com rastreabilidade |
| Embalagem íntegra? | Sim/Não | Sim | |
| Acessórios incluídos? | Sim/Não/Não se aplica | Sim | Quando houver acessórios |
| Pedido identificado fisicamente? | Sim/Não | Sim | Nome, produto, quantidade, destino |
| Divergência de estoque? | Sim/Não | Sim | |
| Descrição da divergência | Texto longo | Condicional | Se houver divergência |

---

# 6. Bloco: Conferência Antes da Saída

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Conferência realizada? | Sim/Não | Sim | |
| Responsável pela conferência | Texto | Sim | |
| Data/hora da conferência | Data/Hora | Sim | |
| Pedido conferido contra CRM/pedido? | Sim/Não | Sim | |
| Endereço conferido? | Sim/Não | Sim | |
| Recebedor conferido? | Sim/Não | Sim | |
| Pagamento/condição validado? | Sim/Não/Não se aplica | Sim | |
| NF/documento anexado? | Sim/Não/Não se aplica | Sim | |
| Pedido liberado para entrega? | Sim/Não | Sim | |
| Pendência antes da saída? | Sim/Não | Sim | |
| Descrição da pendência | Texto longo | Condicional | Se houver pendência |

---

# 7. Bloco: Organização da Entrega

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Responsável pela entrega | Texto | Sim | Entregador, motoboy, transportadora ou responsável interno |
| Rota definida? | Sim/Não/Não se aplica | Sim | |
| Cliente comunicado antes da saída? | Sim/Não | Não | Recomendado |
| Pedido saiu para entrega? | Sim/Não | Sim | |
| Data/hora de saída | Data/Hora | Condicional | Obrigatório se saiu para entrega |
| Previsão informada ao cliente? | Sim/Não | Não | |
| Canal de comunicação | Lista | Não | WhatsApp / Ligação / E-mail / Outro |
| Observação logística | Texto longo | Não | |

---

# 8. Bloco: Entrega e Comprovação

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Status da entrega | Lista | Sim | Entregue / Cliente ausente / Endereço incorreto / Entrega parcial / Produto recusado / Pagamento pendente / Reagendada / Ocorrência aberta / Devolvido |
| Data/hora da entrega | Data/Hora | Condicional | Obrigatório se entregue |
| Quem recebeu | Texto | Condicional | Obrigatório se entregue |
| Produto entregue corretamente? | Sim/Não/Parcial | Sim | |
| Quantidade entregue corretamente? | Sim/Não/Parcial | Sim | |
| Comprovante de entrega obtido? | Sim/Não | Sim | |
| Tipo de comprovante | Lista | Condicional | Assinatura / Foto / WhatsApp / Nome do recebedor / Documento institucional / Outro |
| Comprovante anexado | Upload ou link | Recomendado | Foto, print, comprovante assinado |
| Cliente confirmou recebimento? | Sim/Não | Não | |
| Observações da entrega | Texto longo | Não | |

---

# 9. Bloco: Ocorrências

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Houve ocorrência? | Sim/Não | Sim | |
| Tipo de ocorrência | Lista | Condicional | Atraso / Produto errado / Quantidade divergente / Cliente ausente / Endereço incorreto / Produto avariado / Pagamento pendente / Devolução / Troca / Outro |
| Descrição da ocorrência | Texto longo | Condicional | Detalhar o problema |
| Cliente comunicado? | Sim/Não | Condicional | Obrigatório se houver ocorrência |
| Responsável pela correção | Texto | Condicional | Obrigatório se houver ocorrência |
| Prazo de correção | Data | Condicional | Obrigatório se houver ocorrência |
| Ação corretiva definida | Texto longo | Condicional | |
| Status da ocorrência | Lista | Condicional | Aberta / Em tratamento / Resolvida / Cancelada |
| Ocorrência resolvida? | Sim/Não | Condicional | |
| Data de resolução | Data | Condicional | Se resolvida |

---

# 10. Bloco: Fechamento Operacional

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Status final da C7 | Lista | Sim | Entregue e concluído / Entregue com ocorrência resolvida / Entrega pendente / Reentrega programada / Entrega parcial / Devolvido / Cancelado / Recorrência criada |
| CRM atualizado? | Sim/Não | Sim | Gate de conclusão |
| Comercial informado? | Sim/Não/Não se aplica | Não | Quando necessário |
| Financeiro informado? | Sim/Não/Não se aplica | Não | Quando necessário |
| Estoque ajustado? | Sim/Não/Não se aplica | Não | Quando houver divergência, devolução ou troca |
| Próximo passo operacional | Texto longo | Sim | Mesmo que seja “nenhum” |
| Responsável pelo próximo passo | Texto | Condicional | Se houver próximo passo |
| Data de follow-up operacional | Data | Condicional | Se houver pendência |

---

# 11. Bloco: Recorrência

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Recorrência identificada? | Sim/Não | Sim | |
| Recorrência criada? | Sim/Não | Condicional | Obrigatório se recorrência identificada |
| Frequência de recompra | Lista | Condicional | Semanal / Quinzenal / Mensal / Outro |
| Quantidade prevista por ciclo | Número | Condicional | |
| Data prevista da próxima compra | Data | Condicional | |
| Responsável pelo acompanhamento | Texto | Condicional | |
| Cliente aceitou lembrete de recompra? | Sim/Não | Não | |
| Observação sobre consumo/recompra | Texto longo | Não | |

---

# 12. Regras de Uso do Formulário

## Regra 1 — Não separar pedido incompleto

Não iniciar separação se faltar:

- produto;
- quantidade;
- pagamento ou condição autorizada;
- endereço;
- responsável pelo recebimento.

---

## Regra 2 — Não enviar sem conferência

Todo pedido deve passar por conferência antes da saída.

---

## Regra 3 — Produto inadequado não sai

Produto vencido, avariado, violado, com embalagem danificada ou condição duvidosa deve ser bloqueado e registrado como ocorrência.

---

## Regra 4 — Entrega precisa de comprovação

Toda entrega deve ter algum comprovante:

- assinatura;
- foto;
- confirmação por WhatsApp;
- nome de quem recebeu;
- registro do entregador;
- documento institucional.

---

## Regra 5 — Ocorrência precisa de responsável

Toda ocorrência deve ter:

- tipo;
- descrição;
- responsável;
- prazo;
- status;
- ação corretiva.

---

## Regra 6 — CRM deve ser atualizado

A C7 não termina sem status final atualizado no CRM.

---

## Regra 7 — Recorrência precisa virar tarefa

Se a venda for recorrente, criar:

- frequência;
- próxima data de compra;
- responsável pelo acompanhamento.

---

## Regra 8 — Promessa operacional precisa ser validada

Não prometer urgência, prazo especial, entrega fora de rota, reserva ou substituição sem validação interna.

---

# 13. Versão Mínima para Implantação Inicial

Caso o CRM precise começar de forma mais simples, usar inicialmente apenas os campos abaixo:

| Campo | Tipo | Obrigatório |
|------|------|------------|
| Pedido recebido | Sim/Não | Sim |
| Produto | Texto | Sim |
| Quantidade | Número | Sim |
| Pagamento/condição validado | Sim/Não/Não se aplica | Sim |
| Endereço confirmado | Sim/Não | Sim |
| Responsável pelo recebimento | Texto | Sim |
| Produto separado | Sim/Não | Sim |
| Conferência realizada | Sim/Não | Sim |
| Data prevista de entrega | Data | Sim |
| Status da entrega | Lista | Sim |
| Quem recebeu | Texto | Condicional |
| Comprovante obtido | Sim/Não | Sim |
| Houve ocorrência | Sim/Não | Sim |
| Status final da C7 | Lista | Sim |
| Recorrência criada | Sim/Não | Condicional |
| Data da próxima recompra | Data | Condicional |

---

# 14. Resultado Esperado

Com este formulário, a Santa Luzia passa a ter uma C7 mais controlada, reduzindo:

- erro de produto;
- erro de quantidade;
- entrega sem confirmação;
- ocorrência sem dono;
- perda de histórico operacional;
- retrabalho;
- divergência de estoque;
- falha de comunicação;
- perda de recorrência.

O formulário também melhora:

- experiência do cliente;
- rastreabilidade;
- qualidade da entrega;
- previsibilidade operacional;
- controle de ocorrências;
- integração entre comercial, estoque, logística e pós-venda.
