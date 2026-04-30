# C6 — PROPOSTA, NEGOCIAÇÃO E FECHAMENTO  
## Versão Redesenhada e Otimizada

**Área:** Comercial  
**Etapa:** C6  
**Nome da etapa:** Proposta, Negociação e Fechamento  
**Base utilizada:** leitura da etapa C6 na fonte + pesquisa profunda de mercado sobre proposta, negociação, compras em saúde, home care, nutrição enteral e distribuição de produtos médicos  
**Status:** proposta de redesenho para validação antes de virar SOP final  

---

# 1. Contexto do redesenho

A etapa C6, conforme definida na fonte, é o momento em que a oportunidade passa pela apresentação da proposta, negociação e fechamento da venda.

Na estrutura atual, a C6 já possui uma lógica correta:

- apresentar proposta;
- validar entendimento do cliente;
- negociar, quando necessário;
- confirmar fechamento;
- encaminhar internamente para execução.

Porém, a pesquisa de mercado mostrou que, em empresas mais maduras do segmento de saúde, nutrição enteral, home care e distribuição de produtos médicos, essa etapa precisa ser mais controlada.

A C6 não deve ser apenas “enviar orçamento” ou “negociar preço”. Ela deve funcionar como um processo de:

- formalização da solução;
- validação final dos dados;
- controle de negociação;
- preservação de margem;
- documentação;
- conversão em pedido;
- preparação da entrega;
- criação de recorrência, quando aplicável.

---

# 2. Problemas que o redesenho busca resolver

A C6 sem estrutura pode gerar:

- proposta enviada com dados incompletos;
- orçamento feito sem validação da C4;
- negociação baseada apenas em preço;
- desconto concedido sem critério;
- perda de margem;
- falta de controle sobre validade da proposta;
- proposta enviada e esquecida;
- falta de follow-up;
- fechamento sem dados de entrega;
- pedido confirmado sem pagamento ou documento;
- perda de venda recorrente;
- dependência excessiva de WhatsApp;
- ausência de histórico no CRM;
- falta de motivo claro de perda.

O redesenho corrige esses pontos transformando a C6 em uma etapa com substatus, regras, campos obrigatórios e saídas claras.

---

# 3. Nova definição da C6

> **C6 é a etapa de formalização da proposta, negociação controlada e conversão da oportunidade em pedido, garantindo que produto, quantidade, preço, documentação, pagamento, entrega e próximo passo estejam validados antes da execução operacional.**

---

# 4. Papel da C6 dentro do funil

A C6 é o ponto de conversão da oportunidade em receita.

Ela recebe dados das etapas anteriores:

- **C4:** produto, quantidade, necessidade, logística, pagador, tipo de venda e recorrência;
- **C5:** objeções, comparações, barreiras, necessidade de desconto ou escalonamento.

A C6 deve entregar para a etapa seguinte:

- pedido fechado;
- pagamento ou condição definida;
- dados de entrega confirmados;
- documentos necessários organizados;
- recorrência programada, quando houver;
- registro completo no CRM;
- motivo de perda, se a venda não avançar.

---

# 5. Princípios do novo desenho

## 5.1 Proposta nasce de dados validados

A proposta não deve ser criada com base em mensagem solta, memória ou interpretação incompleta.

Ela deve nascer dos dados registrados na C4 e, quando houver, da C5.

## 5.2 Negociação não começa com desconto

Antes de conceder desconto, a equipe deve entender:

- o que está sendo comparado;
- se o produto é o mesmo;
- se a quantidade é a mesma;
- se a entrega está inclusa;
- se existe concorrente;
- se o cliente está comparando valor total ou apenas preço unitário;
- qual impacto na margem.

## 5.3 Toda proposta tem validade

Toda proposta deve ter data de validade para evitar uso de orçamento antigo, preço desatualizado ou condição que não pode mais ser mantida.

## 5.4 Toda C6 termina com status e próximo passo

A C6 não pode terminar como “cliente ficou de ver”.

Ela deve terminar com uma saída objetiva:

- pedido fechado;
- em negociação;
- aguardando pagamento;
- aguardando documento;
- recorrência programada;
- perdida;
- desqualificada;
- follow-up agendado.

## 5.5 O CRM é o registro oficial

O WhatsApp pode ser usado como canal de comunicação e envio de proposta, mas o CRM deve registrar:

- valor;
- data de envio;
- validade;
- status;
- negociação;
- desconto;
- próximo passo;
- follow-up;
- motivo de perda, se houver.

---

# 6. Estrutura redesenhada da C6

A nova C6 passa a ser composta por cinco blocos:

1. **C6.1 — Preparação da proposta**
2. **C6.2 — Envio da proposta**
3. **C6.3 — Validação de entendimento**
4. **C6.4 — Negociação controlada**
5. **C6.5 — Fechamento ou encaminhamento**

---

# 7. C6.1 — Preparação da proposta

## Objetivo

Garantir que a proposta seja montada com dados completos e coerentes com o que foi validado nas etapas anteriores.

## Quem executa

Responsável comercial pela oportunidade.

## Entradas necessárias

Antes de preparar a proposta, verificar se existem:

- cliente identificado;
- responsável pela decisão;
- responsável pelo pagamento;
- produto validado;
- quantidade estimada;
- tipo de venda: pontual, recorrente ou institucional;
- endereço ou forma de entrega;
- condição de pagamento provável;
- status da prescrição ou documento, quando aplicável;
- existência de objeção registrada;
- necessidade de proposta formal ou orçamento simples;
- estoque ou disponibilidade estimada.

## Regra de entrada

A proposta não deve ser preparada se faltarem dados críticos:

- produto;
- quantidade;
- pagador;
- forma de entrega;
- condição comercial mínima;
- responsável pela decisão.

Se os dados estiverem incompletos, a oportunidade deve retornar para C4 ou permanecer pendente com tarefa definida.

## Checklist de preparação

- [ ] Produto validado
- [ ] Quantidade definida
- [ ] Pagador identificado
- [ ] Responsável pela decisão identificado
- [ ] Entrega viável
- [ ] Condição de pagamento prevista
- [ ] Documento/prescrição conferido, quando aplicável
- [ ] Objeções anteriores verificadas
- [ ] Estoque/disponibilidade verificado, quando necessário
- [ ] Tipo de proposta definido

---

# 8. C6.2 — Envio da proposta

## Objetivo

Formalizar a solução para o cliente de maneira clara, rastreável e comparável.

## Formatos possíveis

A proposta pode ser enviada por:

- WhatsApp;
- PDF;
- e-mail;
- mensagem estruturada;
- orçamento formal;
- documento institucional.

O canal pode variar, mas o conteúdo mínimo deve ser mantido.

## Conteúdo mínimo da proposta

Toda proposta deve conter:

- nome do cliente ou instituição;
- produto;
- apresentação, quando aplicável;
- quantidade;
- valor unitário;
- valor total;
- condição de pagamento;
- prazo ou condição de entrega;
- validade da proposta;
- observações importantes;
- próximos passos para fechar.

## Regras de envio

- Toda proposta enviada deve ser registrada no CRM.
- Toda proposta deve ter validade.
- Toda proposta deve ter follow-up definido.
- Toda condição especial precisa ser registrada.
- Proposta institucional deve ter mais formalidade que proposta para familiar/cuidador.

## Exemplo de mensagem simples para WhatsApp

> Conforme validado, segue orçamento referente a [produto/quantidade].  
> Valor total: R$ [valor].  
> Condição de pagamento: [condição].  
> Entrega: [prazo/condição].  
> Validade da proposta: até [data].  
> Para seguirmos, preciso da confirmação do pedido e do pagamento/dados necessários.

---

# 9. C6.3 — Validação de entendimento

## Objetivo

Confirmar se o cliente entendeu a proposta antes de iniciar qualquer negociação.

## Por que esta etapa existe

Muitas objeções de preço surgem por comparação incorreta:

- produto diferente;
- marca diferente;
- apresentação diferente;
- quantidade diferente;
- entrega inclusa em uma proposta e não em outra;
- compra pontual comparada com recorrência;
- prazo diferente;
- condição de pagamento diferente.

## Perguntas recomendadas

Antes de negociar, perguntar:

- A proposta ficou clara?
- O produto e a quantidade estão corretos?
- O prazo de entrega atende?
- A forma de pagamento atende?
- Existe alguma informação faltando?
- Você está comparando com outra proposta?
- A comparação é do mesmo produto e mesma quantidade?
- O que falta para fecharmos?
- Quem mais precisa aprovar?

## Resultado esperado

Ao final da validação, a equipe deve saber se:

- o cliente entendeu a proposta;
- existe objeção real;
- a negociação é sobre preço, prazo, pagamento, entrega, documento ou decisão;
- a proposta pode seguir para fechamento;
- C5 precisa ser acionada.

---

# 10. C6.4 — Negociação controlada

## Objetivo

Negociar sem improviso, preservando margem e mantendo coerência com os dados validados.

## Tipos de negociação

A negociação pode envolver:

- preço;
- desconto;
- prazo de pagamento;
- forma de pagamento;
- prazo de entrega;
- volume;
- recorrência;
- composição do pedido;
- condição institucional;
- validade da proposta;
- taxa de entrega;
- reserva de produto.

## Regra principal

> Desconto não é a primeira resposta. Desconto é uma possibilidade depois de diagnóstico.

## Antes de conceder desconto, registrar

- motivo do pedido de desconto;
- comparação utilizada pelo cliente;
- produto comparado;
- quantidade comparada;
- preço concorrente, se informado;
- impacto na margem;
- aprovação necessária;
- validade da condição especial.

## Alternativas ao desconto

Sempre avaliar antes de reduzir preço:

- ajustar volume;
- oferecer condição para compra recorrente;
- propor pedido inicial menor;
- alterar forma de pagamento;
- ajustar prazo de entrega;
- separar itens essenciais de complementares;
- criar condição por quantidade;
- oferecer segunda compra programada;
- manter preço e reforçar entrega/segurança/disponibilidade.

## Quando acionar C5

A C5 deve ser acionada dentro da C6 quando surgir:

- objeção de preço;
- comparação com concorrente;
- fornecedor atual;
- falta de orçamento;
- insegurança;
- decisor ausente;
- documentação pendente;
- contrato/política;
- objeção logística.

## Quando escalar

Escalar para o dono/responsável superior quando houver:

- cliente institucional relevante;
- desconto fora da regra;
- risco de margem;
- contrato/política;
- condição especial relevante;
- conflito com fornecedor atual;
- grande volume;
- risco operacional;
- decisão estratégica.

---

# 11. C6.5 — Fechamento ou encaminhamento

## Objetivo

Transformar a decisão do cliente em ação operacional clara.

## Saídas possíveis da C6

### 1. Pedido fechado

Usar quando:

- cliente confirmou a compra;
- produto e quantidade estão definidos;
- pagamento ou condição foi definida;
- entrega está validada;
- dados estão completos.

Próximo passo:

- registrar pedido;
- acionar estoque/separação;
- acionar entrega;
- registrar data prevista;
- criar recorrência, quando aplicável.

---

### 2. Proposta em negociação

Usar quando:

- cliente ainda está avaliando;
- existe ajuste de preço, prazo ou pagamento;
- há comparação em andamento;
- existe necessidade de retorno.

Próximo passo:

- registrar ponto pendente;
- criar follow-up;
- definir responsável;
- registrar prazo de retorno.

---

### 3. Aguardando pagamento

Usar quando:

- cliente confirmou, mas ainda não pagou;
- venda depende de comprovante;
- pagamento será feito em momento combinado.

Próximo passo:

- registrar forma de pagamento;
- acompanhar comprovante;
- definir prazo limite;
- não liberar entrega sem regra interna cumprida.

---

### 4. Aguardando documento

Usar quando:

- falta prescrição;
- falta cadastro;
- falta empenho;
- falta autorização;
- falta dados de NF;
- falta aprovação interna do cliente.

Próximo passo:

- registrar documento pendente;
- solicitar ao cliente;
- criar follow-up.

---

### 5. Recorrência programada

Usar quando:

- consumo contínuo foi confirmado;
- frequência de compra é previsível;
- cliente aceitou acompanhamento;
- próxima compra pode ser antecipada.

Próximo passo:

- registrar frequência;
- criar data de recompra;
- definir responsável pelo acompanhamento.

---

### 6. Perdida

Usar quando:

- cliente não avançou;
- comprou de concorrente;
- preço foi impeditivo;
- prazo/logística não atendeu;
- não houve orçamento;
- desistiu;
- não respondeu após tentativas definidas.

Próximo passo:

- registrar motivo de perda;
- registrar concorrente, se souber;
- encerrar ou colocar em nutrição futura, se fizer sentido.

---

### 7. Desqualificada

Usar quando:

- produto não é fornecido;
- venda é inviável;
- cliente não possui condição de compra;
- risco de atuação fora do escopo;
- documentação obrigatória não será apresentada;
- logística inviável.

Próximo passo:

- registrar motivo;
- encerrar com justificativa.

---

# 12. Substatus recomendados para a C6

Para manter a C6 como uma etapa única, mas com controle interno, recomenda-se usar substatus:

1. Proposta em preparação
2. Proposta enviada
3. Validação de entendimento
4. Em negociação
5. Aguardando pagamento
6. Aguardando documento
7. Pedido fechado
8. Recorrência programada
9. Perdida
10. Desqualificada

---

# 13. Campos recomendados no CRM

## 13.1 Bloco Proposta

- Proposta enviada? Sim/Não
- Data de envio da proposta
- Canal de envio
- Tipo de proposta: simples, recorrente, institucional
- Produto(s)
- Quantidade
- Valor unitário
- Valor total
- Validade da proposta
- Condição de pagamento
- Prazo de entrega
- Observações da proposta

## 13.2 Bloco Validação

- Cliente entendeu a proposta? Sim/Não
- Produto e quantidade confirmados? Sim/Não
- Existe comparação com concorrente? Sim/Não
- Concorrente informado
- O que falta para fechar?
- Decisor final confirmado? Sim/Não

## 13.3 Bloco Negociação

- Houve negociação? Sim/Não
- Tipo de negociação: preço, prazo, pagamento, entrega, volume, recorrência, documentação
- Motivo da negociação
- Desconto solicitado
- Desconto concedido
- Desconto aprovado por quem
- Margem mínima preservada? Sim/Não
- Condição especial concedida
- Validade da condição especial

## 13.4 Bloco Fechamento

- Status da C6
- Próximo passo
- Responsável pelo próximo passo
- Data de follow-up
- Pedido gerado? Sim/Não
- Pagamento confirmado? Sim/Não
- Documento pendente? Sim/Não
- Qual documento pendente?
- Entrega acionada? Sim/Não
- Data prevista de entrega
- Responsável pelo recebimento
- Recorrência criada? Sim/Não
- Frequência de recompra
- Data da próxima recompra

## 13.5 Bloco Perda

- Venda perdida? Sim/Não
- Motivo de perda
- Concorrente escolhido, se conhecido
- Valor perdido
- Observações da perda
- Pode retomar futuramente? Sim/Não
- Data de retomada futura, se aplicável

---

# 14. Regras operacionais da nova C6

## Regra 1 — Não enviar proposta sem dados mínimos

Dados mínimos:

- produto;
- quantidade;
- pagador;
- responsável pela decisão;
- condição de entrega;
- condição de pagamento prevista.

---

## Regra 2 — Toda proposta tem validade

Sem validade, a proposta fica vulnerável a mudança de preço, estoque e condição comercial.

---

## Regra 3 — Toda proposta tem follow-up

Nenhuma proposta pode ficar sem próxima ação.

---

## Regra 4 — Desconto exige diagnóstico

Desconto só pode ocorrer após entender motivo, comparação, impacto e aprovação.

---

## Regra 5 — WhatsApp não substitui CRM

WhatsApp é canal. CRM é registro oficial.

---

## Regra 6 — Promessa operacional precisa ser validada

Não prometer:

- entrega;
- prazo;
- estoque;
- reserva;
- condição especial;
- urgência;

sem confirmar viabilidade.

---

## Regra 7 — Venda recorrente gera agenda

Toda venda recorrente deve gerar data de recompra e responsável pelo acompanhamento.

---

## Regra 8 — Fechamento não é apenas aceite verbal

Para ser considerado fechado, precisa haver:

- confirmação do cliente;
- condição de pagamento;
- dados de entrega;
- próximo passo interno;
- registro no CRM.

---

# 15. Checklist operacional da C6

## Antes de enviar proposta

- [ ] Produto validado
- [ ] Quantidade validada
- [ ] Pagador identificado
- [ ] Decisor identificado
- [ ] Entrega validada
- [ ] Condição de pagamento prevista
- [ ] Prescrição/documento conferido, quando aplicável
- [ ] Estoque/disponibilidade verificado, quando necessário
- [ ] Objeções anteriores revisadas
- [ ] Tipo de proposta definido

## Ao enviar proposta

- [ ] Valor unitário informado
- [ ] Valor total informado
- [ ] Condição de pagamento informada
- [ ] Prazo de entrega informado
- [ ] Validade informada
- [ ] Próximo passo informado ao cliente
- [ ] Proposta registrada no CRM
- [ ] Follow-up criado

## Antes de negociar

- [ ] Cliente entendeu a proposta
- [ ] Produto comparado é o mesmo
- [ ] Quantidade comparada é a mesma
- [ ] Entrega foi considerada
- [ ] Objeção foi classificada
- [ ] C5 acionada, se necessário

## Antes de fechar

- [ ] Pedido confirmado
- [ ] Pagamento/condição definido
- [ ] Documento pendente resolvido ou registrado
- [ ] Dados de entrega confirmados
- [ ] Responsável pelo recebimento definido
- [ ] Estoque/entrega acionado
- [ ] Recorrência criada, se aplicável

---

# 16. Indicadores sugeridos

Para acompanhar a qualidade da C6:

- número de propostas enviadas;
- taxa de conversão proposta → pedido;
- valor total proposto;
- valor total fechado;
- ticket médio;
- tempo médio entre proposta e fechamento;
- percentual de propostas com follow-up em dia;
- percentual de propostas vencidas;
- percentual de propostas perdidas por preço;
- percentual médio de desconto;
- propostas com desconto sem aprovação;
- perda por falta de documento;
- perda por prazo/logística;
- propostas aguardando pagamento;
- propostas aguardando documento;
- recorrências criadas na C6;
- vendas perdidas por ausência de follow-up.

---

# 17. Versão mínima viável

Para implantação rápida, a C6 pode começar com os seguintes campos obrigatórios:

- proposta enviada;
- data de envio;
- valor total;
- validade da proposta;
- status da C6;
- houve negociação;
- houve desconto;
- próximo passo;
- responsável;
- data de follow-up;
- pedido fechado;
- motivo de perda, se aplicável;
- recorrência criada, se aplicável.

---

# 18. Versão ideal futura

Em uma versão mais madura, a C6 pode evoluir para:

- modelo padronizado de proposta;
- automação de follow-up;
- alerta de proposta vencida;
- controle de desconto por aprovação;
- integração com estoque;
- integração com financeiro;
- geração automática de pedido;
- agenda automática de recompra;
- painel de conversão por tipo de cliente;
- análise de perda por motivo;
- histórico de negociação por cliente.

---

# 19. Pontos de decisão do dono

## 19.1 Desconto terá regra de aprovação?

Sugestão: sim.  
Mesmo que manual no início, desconto precisa de critério.

## 19.2 Toda proposta terá validade?

Sugestão: sim.  
A validade deve ser obrigatória.

## 19.3 WhatsApp pode continuar como canal?

Sugestão: sim.  
Mas CRM deve ser o registro oficial.

## 19.4 C6 será etapa única ou separada em proposta e negociação?

Sugestão: manter como etapa única com substatus internos.

## 19.5 Toda recorrência terá lembrete?

Sugestão: sim.  
A recorrência é uma das maiores oportunidades de ganho da Santa Luzia.

---

# 20. Conclusão

A C6 redesenhada transforma a etapa de negociação em um processo controlado de conversão.

Ela deixa de ser apenas:

> “enviar orçamento e esperar resposta”

e passa a ser:

> **formalizar a solução, controlar a negociação, proteger margem, fechar com segurança e preparar a execução operacional.**

O principal ganho esperado é aumentar conversão sem perder margem e sem comprometer a operação.

A nova C6 conecta diretamente:

- dados da C4;
- objeções da C5;
- proposta da C6;
- pedido;
- entrega;
- recorrência.

Com isso, a Santa Luzia passa a ter uma etapa de fechamento mais previsível, rastreável e escalável.
