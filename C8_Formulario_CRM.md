# FORMULÁRIO CRM — C8 PÓS-VENDA, ACOMPANHAMENTO, SATISFAÇÃO E RECORRÊNCIA

## 1. Objetivo do Formulário

Padronizar o registro da etapa C8 no CRM, garantindo que o pós-venda seja executado de forma rastreável, com controle de satisfação, tratamento de problemas e ativação de recorrência.

Este formulário deve apoiar:

- contato pós-entrega;
- confirmação de recebimento;
- verificação de satisfação;
- identificação de problemas;
- acionamento de correções;
- registro de feedback;
- criação de recompra;
- relacionamento contínuo;
- geração de novas oportunidades.

---

# 2. Bloco: Gatilho do Pós-venda

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Pós-venda necessário? | Sim/Não | Sim | Gate inicial da C8 |
| Motivo do pós-venda | Lista | Sim | Primeira compra / Venda recorrente / Ocorrência na C7 / Cliente institucional / Alto valor / Indicação / Outro |
| Tipo de pós-venda | Lista | Sim | Mínimo / Completo |
| Data prevista do contato | Data | Sim | |
| Responsável pelo contato | Texto | Sim | Pessoa responsável por executar a C8 |
| Canal previsto | Lista | Sim | WhatsApp / Ligação / E-mail / Presencial / Outro |
| Cliente é recorrente? | Sim/Não | Sim | Ajuda a definir prioridade |
| Houve ocorrência na C7? | Sim/Não | Sim | Se sim, acompanhar até resolução |
| Observações da C7 | Texto longo | Não | Informações relevantes da entrega |

---

# 3. Bloco: Contato Pós-entrega

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Contato realizado? | Sim/Não | Sim | |
| Data do contato | Data | Condicional | Obrigatório se contato realizado |
| Horário do contato | Hora | Não | |
| Canal utilizado | Lista | Condicional | WhatsApp / Ligação / E-mail / Presencial / Outro |
| Cliente respondeu? | Sim/Não | Sim | |
| Número da tentativa | Número | Sim | Ex.: 1, 2, 3 |
| Próxima tentativa necessária? | Sim/Não | Condicional | Se cliente não respondeu |
| Data da próxima tentativa | Data | Condicional | Se houver nova tentativa |
| Mensagem enviada registrada? | Sim/Não | Não | Print/link/anotação |
| Resumo do contato | Texto longo | Não | |

---

# 4. Bloco: Confirmação da Entrega

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Pedido chegou corretamente? | Sim/Não/Não respondeu | Sim | |
| Produto correto? | Sim/Não/Não respondeu | Sim | |
| Quantidade correta? | Sim/Não/Não respondeu | Sim | |
| Entrega ocorreu no prazo? | Sim/Não/Não respondeu | Sim | |
| Entrega foi satisfatória? | Sim/Não/Parcial/Não respondeu | Sim | |
| Houve divergência na entrega? | Sim/Não | Sim | |
| Descrição da divergência | Texto longo | Condicional | Obrigatório se houve divergência |
| Cliente confirmou recebimento? | Sim/Não/Não respondeu | Sim | |
| Comentário sobre entrega | Texto longo | Não | |

---

# 5. Bloco: Satisfação do Cliente

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Satisfação geral | Lista | Sim | Satisfeito / Satisfeito com ressalva / Insatisfeito / Não respondeu / Problema aberto |
| Comentário do cliente | Texto longo | Não | Registrar fala relevante |
| Cliente indicaria a empresa? | Sim/Não/Não perguntado | Não | Pode ser usado como indicador simples |
| Nota de satisfação | Número | Não | Opcional, escala interna |
| Principal ponto positivo | Texto | Não | |
| Principal ponto negativo | Texto | Não | |
| Cliente demonstrou confiança para comprar novamente? | Sim/Não/Indefinido | Não | |

---

# 6. Bloco: Problemas e Ocorrências

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Houve problema? | Sim/Não | Sim | |
| Tipo de problema | Lista | Condicional | Atraso / Produto incorreto / Quantidade divergente / Embalagem danificada / Dúvida operacional / Atendimento / Cobrança / Troca / Devolução / Outro |
| Descrição do problema | Texto longo | Condicional | Detalhar o ocorrido |
| Problema veio da C7? | Sim/Não/Não identificado | Não | Ajuda na melhoria do processo |
| Problema veio da C6? | Sim/Não/Não identificado | Não | Ex.: proposta/pagamento/condição mal alinhada |
| Problema veio da C4? | Sim/Não/Não identificado | Não | Ex.: produto/quantidade mal validados |
| Necessita correção? | Sim/Não | Condicional | |
| Responsável pela correção | Texto | Condicional | Obrigatório se houver problema |
| Prazo de correção | Data | Condicional | Obrigatório se houver problema |
| Status do problema | Lista | Condicional | Aberto / Em tratamento / Resolvido / Cancelado |
| Retorno dado ao cliente? | Sim/Não | Condicional | Obrigatório se houver problema |
| Problema resolvido? | Sim/Não | Condicional | |
| Data de resolução | Data | Condicional | Se resolvido |
| Ação corretiva aplicada | Texto longo | Não | |

---

# 7. Bloco: Dúvidas e Limite de Escopo

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Cliente apresentou dúvida? | Sim/Não | Sim | |
| Tipo de dúvida | Lista | Condicional | Compra / Entrega / Reposição / Armazenamento / Pagamento / Produto / Clínica / Outro |
| Descrição da dúvida | Texto longo | Condicional | |
| Dúvida dentro do escopo comercial? | Sim/Não | Condicional | |
| Foi necessário encaminhar para profissional responsável? | Sim/Não | Condicional | Para dúvida clínica |
| Encaminhamento realizado? | Sim/Não/Não se aplica | Condicional | |
| Observação sobre encaminhamento | Texto longo | Não | |

---

# 8. Bloco: Recorrência e Recompra

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Há potencial de recorrência? | Sim/Não | Sim | |
| Recorrência confirmada? | Sim/Não | Condicional | Obrigatório se houver potencial |
| Tipo de recorrência | Lista | Condicional | Semanal / Quinzenal / Mensal / Sob demanda / Outro |
| Frequência de recompra | Lista | Condicional | Semanal / Quinzenal / Mensal / Outro |
| Quantidade prevista por ciclo | Número | Condicional | |
| Data provável da próxima compra | Data | Condicional | |
| Cliente aceitou lembrete de recompra? | Sim/Não | Condicional | |
| Responsável pela recompra | Texto | Condicional | |
| Canal preferido para recompra | Lista | Não | WhatsApp / Ligação / E-mail / Outro |
| Prescrição continua a mesma? | Sim/Não/Não informado/Não se aplica | Condicional | Importante para produtos com prescrição |
| Houve mudança de produto ou quantidade? | Sim/Não/Não informado | Não | |
| Observação sobre consumo/recompra | Texto longo | Não | |

---

# 9. Bloco: Relacionamento e Oportunidades Futuras

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Cliente satisfeito para indicação? | Sim/Não/Indefinido | Não | |
| Origem da indicação | Texto | Não | Se aplicável |
| Nutricionista/prescritor relacionado | Texto | Não | Se houver |
| Oportunidade futura identificada? | Sim/Não | Sim | |
| Tipo de oportunidade futura | Lista | Condicional | Recompra / Produto complementar / Novo paciente / Indicação / Institucional / Outro |
| Descrição da oportunidade futura | Texto longo | Condicional | |
| Nova oportunidade criada no CRM? | Sim/Não/Não se aplica | Condicional | |
| Próximo contato de relacionamento | Data | Não | |
| Observações de relacionamento | Texto longo | Não | |

---

# 10. Bloco: Encerramento da C8

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Status final da C8 | Lista | Sim | Cliente satisfeito / Cliente satisfeito com recorrência / Problema aberto / Problema resolvido / Não respondeu / Nova oportunidade criada / Encerrado sem ação |
| Próximo passo | Texto longo | Sim | Nenhuma C8 deve encerrar sem definição |
| Responsável pelo próximo passo | Texto | Condicional | Obrigatório se houver próximo passo |
| Data de follow-up | Data | Condicional | Obrigatório se houver próxima ação |
| CRM atualizado? | Sim/Não | Sim | Gate de conclusão |
| Comercial informado? | Sim/Não/Não se aplica | Não | Quando houver oportunidade, problema ou recorrência |
| Operação/C7 informada? | Sim/Não/Não se aplica | Não | Quando houver problema de entrega |
| Observações finais | Texto longo | Não | |

---

# 11. Regras de Uso do Formulário

## Regra 1 — Toda primeira compra gera pós-venda

A primeira compra deve gerar contato obrigatório, preferencialmente em até 24–48 horas após a entrega.

## Regra 2 — Toda venda recorrente gera lembrete

Se houver recorrência, devem ser preenchidos:

- frequência de recompra;
- data provável da próxima compra;
- responsável pela recompra;
- canal preferido, quando possível.

## Regra 3 — Todo problema gera responsável e prazo

Se houver problema, não basta registrar. É obrigatório definir:

- tipo de problema;
- descrição;
- responsável;
- prazo;
- status;
- retorno ao cliente.

## Regra 4 — WhatsApp é canal, CRM é registro

O contato pode acontecer pelo WhatsApp, mas o CRM deve guardar o histórico oficial da C8.

## Regra 5 — Dúvida clínica deve ser encaminhada

A equipe não deve orientar troca de dieta, volume, frequência, prescrição ou conduta clínica.

Quando a dúvida for clínica, registrar e orientar o cliente a procurar o profissional responsável.

## Regra 6 — Cliente sem resposta tem limite de tentativas

Sugestão inicial:

1. primeira tentativa: até 24–48h após entrega;
2. segunda tentativa: após 2 dias;
3. terceira tentativa: após 5 a 7 dias;
4. depois classificar como “não respondeu”.

## Regra 7 — Feedback recorrente vira melhoria de processo

Problemas repetidos devem ser usados para revisar etapas anteriores:

- atraso frequente → revisar C7;
- erro de produto → revisar C6/C7;
- dúvida de quantidade → revisar C4/C6;
- reclamação de preço na recompra → revisar C5/C6;
- perda de recompra → revisar C8.

---

# 12. Versão Mínima para Implantação Inicial

Caso o CRM precise começar de forma mais simples, usar inicialmente apenas os campos abaixo:

| Campo | Tipo | Obrigatório |
|------|------|------------|
| Pós-venda necessário | Sim/Não | Sim |
| Data prevista de contato | Data | Sim |
| Responsável pelo contato | Texto | Sim |
| Contato realizado | Sim/Não | Sim |
| Cliente respondeu | Sim/Não | Sim |
| Pedido chegou corretamente | Sim/Não/Não respondeu | Sim |
| Satisfação geral | Lista | Sim |
| Houve problema | Sim/Não | Sim |
| Tipo de problema | Lista | Condicional |
| Responsável pela correção | Texto | Condicional |
| Prazo de correção | Data | Condicional |
| Há potencial de recorrência | Sim/Não | Sim |
| Data da próxima compra | Data | Condicional |
| Responsável pela recompra | Texto | Condicional |
| Status final da C8 | Lista | Sim |
| Próximo passo | Texto | Sim |
| CRM atualizado | Sim/Não | Sim |

---

# 13. Resultado Esperado

Com este formulário, a Santa Luzia passa a ter uma C8 mais estruturada, reduzindo:

- perda silenciosa de clientes;
- ausência de recompra;
- problemas sem responsável;
- reclamações sem retorno;
- dependência da memória da equipe;
- falta de histórico no CRM;
- risco de orientação fora do escopo;
- perda de oportunidade futura.

O formulário também melhora:

- satisfação do cliente;
- retenção;
- recompra;
- relacionamento com cuidadores, familiares e instituições;
- controle de problemas;
- qualidade do processo;
- previsibilidade de receita recorrente.
