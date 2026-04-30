# FORMULÁRIO CRM — C9 GESTÃO DE RELACIONAMENTO, RETENÇÃO, RECORRÊNCIA E DESENVOLVIMENTO DA CARTEIRA

## 1. Objetivo do Formulário

Padronizar o registro da etapa C9 no CRM, garantindo que a gestão de relacionamento com clientes seja feita de forma ativa, rastreável e orientada à retenção.

Este formulário deve apoiar:

- segmentação da carteira;
- controle de clientes recorrentes;
- agenda de relacionamento;
- prevenção de perda de clientes;
- reativação de clientes inativos;
- identificação de oportunidades futuras;
- relacionamento com prescritores, home cares e instituições;
- acompanhamento de clientes em risco;
- análise de retenção, recompra e churn.

---

# 2. Bloco: Identificação do Cliente na Carteira

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Cliente incluído na C9? | Sim/Não | Sim | Gate inicial da etapa |
| Nome do cliente/paciente/instituição | Texto | Sim | Deve vir do cadastro/oportunidade |
| Tipo de cliente | Lista | Sim | Familiar / Cuidador / Home Care / Hospital / Clínica / Nutricionista / Institucional / Outro |
| Segmento da carteira | Lista | Sim | Recorrente ativo / Recorrente em risco / Pontual / Institucional / Home Care / Nutricionista-prescritor / Familiar-cuidador / Inativo / Perdido / Parceiro de indicação |
| Status da carteira | Lista | Sim | Ativo recorrente / Ativo pontual / Em acompanhamento / Em risco / Em reativação / Inativo / Perdido / Parceiro ativo |
| Responsável pelo relacionamento | Texto | Sim | Pessoa responsável por acompanhar o cliente |
| Canal preferido de contato | Lista | Não | WhatsApp / Ligação / E-mail / Presencial / Outro |
| Data de entrada na C9 | Data | Sim | |
| Origem do relacionamento | Lista | Não | C8 / Recompra / Indicação / Institucional / Home Care / Outro |
| Observações gerais do cliente | Texto longo | Não | Histórico relevante |

---

# 3. Bloco: Histórico Comercial e Relacionamento

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Data da última compra | Data | Condicional | Obrigatório para clientes compradores |
| Produto principal comprado | Texto | Condicional | Produto mais relevante ou recorrente |
| Valor da última compra | Moeda | Não | |
| Valor mensal estimado | Moeda | Não | Estimativa de potencial recorrente |
| Data do último contato | Data | Sim | |
| Canal do último contato | Lista | Não | WhatsApp / Ligação / E-mail / Presencial / Outro |
| Resumo do último contato | Texto longo | Não | |
| Cliente respondeu ao último contato? | Sim/Não | Não | |
| Satisfação mais recente | Lista | Não | Satisfeito / Satisfeito com ressalva / Insatisfeito / Não respondeu / Problema aberto |
| Houve problema recente? | Sim/Não | Não | |
| Descrição do problema recente | Texto longo | Condicional | Se houve problema |
| Problema resolvido? | Sim/Não/Não se aplica | Não | |

---

# 4. Bloco: Agenda de Relacionamento

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Próximo contato definido? | Sim/Não | Sim | Nenhum cliente ativo deve ficar sem próxima ação |
| Data do próximo contato | Data | Condicional | Obrigatório se próximo contato definido |
| Objetivo do próximo contato | Lista | Condicional | Recompra / Relacionamento / Reativação / Retenção / Indicação / Atualização cadastral / Institucional / Outro |
| Canal previsto | Lista | Não | WhatsApp / Ligação / E-mail / Presencial / Outro |
| Responsável pelo próximo contato | Texto | Condicional | |
| Prioridade do contato | Lista | Não | Alta / Média / Baixa |
| Observação para o próximo contato | Texto longo | Não | |
| Tarefa criada no CRM? | Sim/Não | Sim | |

---

# 5. Bloco: Recorrência e Recompra

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Há potencial de recorrência? | Sim/Não | Sim | |
| Cliente recorrente? | Sim/Não | Sim | |
| Produto recorrente | Texto | Condicional | Obrigatório se recorrente |
| Frequência de recompra | Lista | Condicional | Semanal / Quinzenal / Mensal / Bimestral / Sob demanda / Outro |
| Quantidade por ciclo | Número | Condicional | |
| Data prevista da próxima recompra | Data | Condicional | Obrigatório se recorrente |
| Recompra confirmada? | Sim/Não/Não se aplica | Sim | |
| Status da recompra | Lista | Condicional | Prevista / Confirmada / Adiada / Sem resposta / Em risco / Perdida |
| Cliente ainda usa o mesmo produto? | Sim/Não/Não informado | Condicional | |
| Prescrição continua igual? | Sim/Não/Não informado/Não se aplica | Condicional | |
| Quantidade continua igual? | Sim/Não/Não informado | Condicional | |
| Endereço continua igual? | Sim/Não/Não informado | Não | |
| Risco de ruptura? | Sim/Não | Não | Produto pode acabar antes da próxima compra |
| Data estimada de término do produto | Data | Não | Quando possível estimar |
| Cliente aceitou lembrete? | Sim/Não/Não informado | Não | |
| Observações de recompra | Texto longo | Não | |

---

# 6. Bloco: Risco de Perda

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Cliente em risco? | Sim/Não | Sim | |
| Nível de risco | Lista | Condicional | Baixo / Médio / Alto |
| Motivo do risco | Lista | Condicional | Atraso na recompra / Sem resposta / Reclamação / Preço / Concorrente / Problema de entrega / Queda de volume / Mudança de prescrição / Outro |
| Descrição do risco | Texto longo | Condicional | |
| Data em que risco foi identificado | Data | Condicional | |
| Ação de retenção definida? | Sim/Não | Condicional | |
| Ação de retenção | Texto longo | Condicional | |
| Responsável pela ação | Texto | Condicional | |
| Prazo da ação | Data | Condicional | |
| Status da ação | Lista | Condicional | Aberta / Em andamento / Resolvida / Sem retorno / Perdida |
| Resultado da ação de retenção | Texto longo | Não | |

---

# 7. Bloco: Reativação de Cliente Inativo

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Cliente inativo? | Sim/Não | Sim | |
| Data da última compra antes da inatividade | Data | Condicional | |
| Motivo provável da inatividade | Lista | Condicional | Sem resposta / Comprou de concorrente / Sem necessidade atual / Preço / Problema anterior / Mudança de prescrição / Óbito / Mudança de fornecedor / Outro |
| Régua de reativação iniciada? | Sim/Não | Condicional | |
| Número da tentativa de reativação | Número | Condicional | Ex.: 1, 2, 3 |
| Data da tentativa | Data | Condicional | |
| Canal da tentativa | Lista | Condicional | WhatsApp / Ligação / E-mail / Outro |
| Resultado da tentativa | Lista | Condicional | Respondeu / Não respondeu / Pediu retorno futuro / Comprou novamente / Sem necessidade / Perdido |
| Nova tentativa necessária? | Sim/Não | Condicional | |
| Data da próxima tentativa | Data | Condicional | |
| Cliente reativado? | Sim/Não | Condicional | |
| Classificado como perdido? | Sim/Não | Condicional | |
| Observações da reativação | Texto longo | Não | |

---

# 8. Bloco: Desenvolvimento de Oportunidades

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Oportunidade futura identificada? | Sim/Não | Sim | |
| Tipo de oportunidade | Lista | Condicional | Recompra / Produto complementar / Aumento de volume / Novo paciente / Indicação / Home Care / Institucional / Contrato recorrente / Outro |
| Descrição da oportunidade | Texto longo | Condicional | |
| Potencial de valor | Moeda | Não | Estimativa, quando possível |
| Nova oportunidade criada no CRM? | Sim/Não/Não se aplica | Condicional | |
| Etapa indicada no funil | Lista | Condicional | C4 / C5 / C6 / C7 / Recompra simples / Outro |
| Responsável pela nova oportunidade | Texto | Condicional | |
| Data prevista de ação comercial | Data | Condicional | |
| Observações comerciais | Texto longo | Não | |

---

# 9. Bloco: Prescritores, Parceiros e Indicações

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Existe prescritor/nutricionista relacionado? | Sim/Não | Não | |
| Nome do prescritor/nutricionista | Texto | Condicional | |
| Existe home care relacionado? | Sim/Não | Não | |
| Nome do home care | Texto | Condicional | |
| Cliente veio por indicação? | Sim/Não | Não | |
| Origem da indicação | Texto | Condicional | |
| Cliente gerou indicação? | Sim/Não | Não | |
| Indicação registrada no CRM? | Sim/Não/Não se aplica | Não | |
| Parceiro ativo? | Sim/Não | Não | Para prescritores, home cares ou instituições |
| Próximo contato com parceiro | Data | Não | |
| Observações de relacionamento com parceiro | Texto longo | Não | |

---

# 10. Bloco: Encerramento ou Atualização do Ciclo C9

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Status final do ciclo C9 | Lista | Sim | Ativo recorrente / Ativo pontual / Em acompanhamento / Em risco / Em reativação / Inativo / Perdido / Nova oportunidade criada |
| Resultado do ciclo | Texto longo | Sim | Resumo do que aconteceu no ciclo atual |
| Próximo passo | Texto longo | Sim | Nenhum ciclo C9 deve encerrar sem definição |
| Responsável pelo próximo passo | Texto | Condicional | |
| Data de follow-up | Data | Condicional | |
| CRM atualizado? | Sim/Não | Sim | Gate de conclusão |
| Cliente deve continuar na C9? | Sim/Não | Sim | |
| Observações finais | Texto longo | Não | |

---

# 11. Regras de Uso do Formulário

## Regra 1 — Todo cliente recorrente deve ter próxima data de contato

Se o cliente tem consumo recorrente, é obrigatório preencher:

- frequência de recompra;
- data prevista da próxima recompra;
- responsável pelo relacionamento;
- próximo contato.

---

## Regra 2 — Cliente atrasado na recompra vira cliente em risco

Se o cliente não recomprar dentro do ciclo esperado, deve ser classificado como “em risco” e gerar ação ativa.

---

## Regra 3 — Cliente inativo precisa ter motivo registrado

Não basta registrar “sumiu”. Deve ser indicado:

- motivo provável;
- tentativas feitas;
- resultado;
- próxima tentativa ou encerramento.

---

## Regra 4 — Nova necessidade vira oportunidade

Quando houver demanda nova, recompra, novo paciente, produto complementar ou indicação, deve ser criada uma oportunidade ou tarefa no CRM.

---

## Regra 5 — Relacionamento com prescritor/parceiro deve ser registrado

Quando houver nutricionista, prescritor, home care ou parceiro de indicação envolvido, o vínculo deve ser registrado para preservar histórico.

---

## Regra 6 — WhatsApp é canal, CRM é registro

Conversas importantes devem ser resumidas no CRM. O histórico oficial da carteira deve ficar no CRM.

---

## Regra 7 — Mudança técnica não segue direto para venda

Se houver mudança de produto, prescrição, volume, frequência ou necessidade técnica, a oportunidade deve voltar para validação antes da venda.

---

## Regra 8 — Clientes em risco têm prioridade semanal

Clientes recorrentes em risco devem aparecer em rotina/lista de prioridade para ação da equipe.

---

# 12. Versão Mínima para Implantação Inicial

Caso o CRM precise começar de forma mais simples, usar inicialmente apenas os campos abaixo:

| Campo | Tipo | Obrigatório |
|------|------|------------|
| Segmento da carteira | Lista | Sim |
| Status da carteira | Lista | Sim |
| Responsável pelo relacionamento | Texto | Sim |
| Produto recorrente | Texto | Condicional |
| Frequência de compra | Lista | Condicional |
| Data da última compra | Data | Condicional |
| Data da próxima recompra | Data | Condicional |
| Próximo contato | Data | Sim |
| Cliente em risco? | Sim/Não | Sim |
| Motivo do risco | Lista | Condicional |
| Cliente inativo? | Sim/Não | Sim |
| Oportunidade futura identificada? | Sim/Não | Sim |
| Próximo passo | Texto | Sim |
| CRM atualizado? | Sim/Não | Sim |

---

# 13. Resultado Esperado

Com este formulário, a Santa Luzia passa a ter uma C9 mais estruturada, reduzindo:

- perda silenciosa de clientes;
- dependência de novos leads;
- falta de controle de recompra;
- clientes recorrentes sem acompanhamento;
- clientes inativos sem tentativa de reativação;
- relacionamento disperso em WhatsApp;
- perda de indicações;
- ausência de previsibilidade da receita;
- falta de histórico de consumo.

O formulário também melhora:

- retenção;
- recompra;
- receita recorrente;
- visão da carteira;
- priorização da equipe;
- identificação de clientes em risco;
- reativação;
- desenvolvimento de oportunidades;
- relacionamento com nutricionistas, home cares e instituições.
