# Canal Home Care — Arquitetura Inicial do CRM

## Objetivo

Criar um módulo específico de Home Care dentro do CRM da Santa Luzia para acompanhar a rede de nutricionistas parceiras e as vendas efetivamente originadas por elas.

## Regra central

A unidade principal de performance é a **venda efetivada**, não a quantidade de prescrições.

Fluxo principal:

`Instituição Home Care -> Nutricionista parceira -> Paciente -> Pedido -> Venda`

Prescrições, quando recebidas no atendimento, podem ser tratadas apenas como documento de apoio ou evidência associada ao pedido, sem formar um funil próprio.

## Entidades principais

### Instituição Home Care

Cadastro próprio para permitir relacionar várias nutricionistas a uma mesma instituição e medir posteriormente o desempenho comercial por instituição.

### Nutricionista parceira

O cadastro deve incluir identificação profissional, contatos, região de atuação, instituição vinculada, status da parceria, histórico de reuniões e indicadores de performance calculados pelo sistema.

### Paciente/cliente

Deve ser vinculado à nutricionista de origem quando essa origem puder ser identificada.

### Pedido

Cada pedido do canal Home Care deve permitir registrar:

- paciente;
- nutricionista de origem;
- instituição de origem, quando aplicável;
- data;
- itens;
- quantidades;
- valores;
- descontos;
- status;
- situação financeira;
- responsável pelo atendimento;
- indicação se a venda é válida para performance.

### Itens do pedido

Devem permitir análise de mix de produtos, quantidade vendida e receita por produto.

### Histórico de relacionamento

Registrar reuniões, contatos, ativações, inativações e próximos passos da nutricionista parceira.

## Status sugerido da nutricionista

`Mapeada -> Contatada -> Reunião agendada -> Reunião realizada -> Parceira -> Ativa -> Inativa`

## Dashboard Home Care

O dashboard deverá acompanhar, entre outros:

- nutricionistas cadastradas;
- nutricionistas parceiras;
- nutricionistas ativas;
- reuniões realizadas;
- novos pacientes compradores;
- vendas do canal;
- receita do canal;
- ticket médio;
- recompras;
- receita recorrente;
- ranking de nutricionistas por receita;
- ranking de nutricionistas por pacientes compradores;
- ranking de instituições Home Care;
- ranking de produtos.

## Atribuição da venda

O CRM deve permitir identificar a nutricionista de origem por mecanismos que ainda serão definidos, incluindo possibilidades como código individual, QR Code, link individual ou identificação manual no atendimento.

## Relatório financeiro

O sistema deve ser capaz de consolidar por período as vendas atribuídas a cada nutricionista, incluindo pedidos válidos, valores, cancelamentos e estornos.

A regra de eventual comissão ou benefício não deve ser fixada na arquitetura até que seja formalmente definida e validada.

## Automações futuras

Possibilidades a avaliar:

- lembretes de reunião;
- follow-up de nutricionistas;
- alerta de nutricionista sem vendas;
- alerta de nova venda atribuída;
- previsão de recompra do paciente;
- alerta de janela de recompra;
- consolidação mensal automática;
- geração de relatórios gerenciais;
- integração com WhatsApp e sistemas de pedidos.

## Próximas definições

Antes da especificação técnica final ainda devem ser definidos:

- fluxo exato do paciente até a compra;
- canais de atendimento;
- mecanismo definitivo de identificação da nutricionista;
- regra para atribuição de recompras;
- definição de venda válida;
- regras para cancelamentos e estornos;
- integração com o sistema de pedidos/faturamento;
- permissões do módulo;
- regras de privacidade e retenção de dados.

## Status

Documento inicial de arquitetura funcional. Banco de dados, APIs, telas e integrações serão especificados depois do fechamento do processo operacional.
