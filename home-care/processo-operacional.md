# Canal Home Care — Processo Operacional

## 1. Objetivo do canal

Criar uma rede escalável de nutricionistas parceiras de Home Care que conheçam os produtos comercializados pela Santa Luzia, identifiquem produtos adequados dentro de sua atuação profissional e direcionem pacientes para compra na empresa, permitindo rastrear as vendas efetivamente originadas por cada parceira.

## 2. Meta inicial de aquisição de nutricionistas

A nutricionista da Santa Luzia deverá realizar reuniões recorrentes com nutricionistas que atuem em Home Care na região.

Meta inicial:

- mínimo de 2 nutricionistas reunidas por semana;
- faixa operacional desejada: 2 a 5 nutricionistas por semana.

As nutricionistas prospectadas geralmente possuem vínculo com empresas ou instituições de Home Care e atendem pacientes dessas instituições.

## 3. Reunião de apresentação

Na reunião, a Santa Luzia apresenta:

- produtos das marcas parceiras, incluindo NVTRO/Nutro e ProDiet;
- características e indicações de uso dos produtos;
- diferenciais técnicos;
- comparação pertinente com soluções concorrentes;
- posicionamento comercial e preços, quando aplicável;
- forma de atendimento ao paciente pela Santa Luzia;
- funcionamento da parceria.

## 4. Conversão em nutricionista parceira

Quando a nutricionista entende o portfólio, considera os produtos adequados para seu contexto profissional e aceita participar do canal, ela passa a ser cadastrada como nutricionista parceira.

O cadastro deverá permitir relacioná-la à instituição ou às instituições de Home Care com as quais possui vínculo.

## 5. Identificação da origem do paciente

A Santa Luzia deverá possuir um mecanismo confiável para identificar qual nutricionista originou cada paciente ou pedido.

A operação poderá utilizar materiais físicos de identificação, como adesivo da Santa Luzia aplicado ao material entregue ao paciente, combinado com mecanismos digitais e/ou códigos únicos.

A definição final do mecanismo de atribuição ainda será detalhada.

## 6. Regra fundamental: pedido/venda é o evento relevante

A quantidade de prescrições emitidas pela nutricionista **não será controlada como KPI nem como etapa operacional relevante do canal**.

O que importa para performance, atribuição e eventual cálculo financeiro é o **pedido efetivamente gerado e convertido em venda**.

Portanto, o fluxo de negócio deve ser modelado como:

`Nutricionista parceira -> paciente originado -> atendimento Santa Luzia -> pedido -> venda efetivada -> atribuição à nutricionista`

Não é necessário criar um funil de prescrições separado.

## 7. Pedido atribuído

Cada pedido originado pelo canal Home Care deverá, sempre que possível, armazenar:

- nutricionista de origem;
- instituição Home Care relacionada;
- paciente/cliente;
- data do pedido;
- itens vendidos;
- quantidade por item;
- valor unitário;
- valor total;
- descontos, quando aplicável;
- status do pedido;
- status financeiro;
- status de venda válida para cálculo de performance/comissionamento;
- responsável pelo atendimento.

## 8. Venda válida

A regra exata para considerar uma venda como válida para performance/comissionamento ainda precisa ser formalizada.

Como princípio de sistema, deve existir diferença entre:

- pedido criado;
- pedido confirmado;
- venda faturada/paga;
- pedido cancelado;
- pedido devolvido ou estornado.

O evento que gera direito financeiro deve ser parametrizável e validado antes da implantação definitiva.

## 9. Recorrência do paciente

Um paciente originado por uma nutricionista poderá realizar múltiplas compras ao longo do tempo.

O sistema deverá permitir medir:

- primeira compra;
- recompras;
- receita acumulada do paciente;
- frequência média de compra;
- última compra;
- próxima janela provável de recompra;
- status de atividade do paciente.

A definição de quais recompras continuam atribuídas à nutricionista de origem dependerá da regra comercial de comissionamento que ainda será definida.

## 10. Funis do canal

### 10.1 Rede de nutricionistas

`Mapeada -> Contatada -> Reunião agendada -> Reunião realizada -> Parceira -> Ativa -> Inativa`

### 10.2 Paciente e venda

`Paciente originado -> Atendimento -> Pedido -> Venda efetivada -> Recompra/Recorrência`

## 11. Indicadores iniciais

Indicadores recomendados para o canal:

### Aquisição da rede

- nutricionistas mapeadas;
- reuniões agendadas;
- reuniões realizadas;
- novas parceiras;
- taxa reunião -> parceria;
- nutricionistas parceiras ativas.

### Geração de negócios

- pacientes originados por nutricionista;
- pedidos gerados por nutricionista;
- vendas efetivadas por nutricionista;
- receita por nutricionista;
- ticket médio;
- margem, quando disponível;
- pacientes com recompra;
- receita recorrente/receita de recompra;
- receita por instituição Home Care.

### Produtos

- produtos vendidos no canal;
- quantidade vendida por produto;
- receita por produto;
- mix por nutricionista;
- mix por instituição Home Care.

## 12. Entidades de negócio principais

A operação deverá tratar como entidades distintas:

- Instituição Home Care;
- Nutricionista parceira;
- Paciente/cliente;
- Pedido;
- Item do pedido;
- Venda/pagamento;
- Regra de atribuição/comissionamento;
- Histórico de relacionamento.

**Prescrição não é uma entidade obrigatória do processo comercial**, pois sua quantidade não é relevante para o objetivo do canal. Caso seja necessário armazenar uma imagem ou documento recebido no atendimento, ele poderá ser tratado apenas como anexo/evidência do pedido, e não como etapa do funil.

## 13. Ponto regulatório e jurídico

Antes de ativar qualquer pagamento, comissão ou benefício diretamente ligado à indicação de pacientes/produtos por profissionais de saúde, a Santa Luzia deverá validar o modelo com assessoria jurídica, compliance e regras profissionais aplicáveis.

O sistema deve ser construído para permitir alterar ou desabilitar regras financeiras sem perder a rastreabilidade comercial das origens das vendas.

## 14. Status deste documento

Versão inicial baseada nas regras já definidas para o novo Canal Home Care. Deve ser atualizada à medida que o processo for detalhado e validado.
