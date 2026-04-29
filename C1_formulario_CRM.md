# Formulário CRM — C1: Captura e Registro de Instituições

**Processo:** C1 — Geração, Captura e Registro de Leads  
**Objetivo do formulário:** padronizar a entrada de instituições no CRM para que o lead siga para C2 com dados mínimos, fonte rastreável e status claro.

---

## 1. Orientação de uso

Este formulário deve ser preenchido sempre que uma nova instituição for capturada para o CRM.

A regra principal é:

> **No C1, a instituição vem antes do contato.**

Não é obrigatório encontrar decisor, comprador, nutricionista ou WhatsApp direto nesta etapa.  
O foco é registrar a instituição corretamente, validar minimamente sua existência e definir se ela pode seguir para triagem no C2.

---

## 2. Bloco A — Identificação da Instituição

### Nome da instituição

**Tipo de campo:** Texto obrigatório  
**Preenchimento:** nome fantasia ou razão social identificável.

**Exemplo:**
```text
Hospital Santa Maria
```

**Regra:**
- Sem nome identificável, não criar lead ativo.
- Evitar abreviações confusas.
- Padronizar nomes duplicados.

---

### Tipo presumido

**Tipo de campo:** Seleção obrigatória

**Opções:**
- OS
- Rede hospitalar
- Hospital
- Home care
- Clínica
- Operadora
- Órgão público
- Outro

**Regra:**
- Usar o tipo mais provável com base na fonte.
- Se houver dúvida, selecionar “Outro” ou “Clínica” e explicar na observação.
- A validação mais profunda será feita no C2.

---

### Município

**Tipo de campo:** Texto obrigatório

**Exemplo:**
```text
Belém
```

**Regra:**
- Usar grafia correta do município.
- Não preencher apenas região ou bairro.

---

### UF

**Tipo de campo:** Seleção obrigatória

**Exemplo:**
```text
PA
```

**Regra:**
- Usar sigla do estado.
- Campo obrigatório para priorização regional.

---

## 3. Bloco B — Origem do Lead

### Fonte do lead

**Tipo de campo:** Seleção obrigatória

**Opções:**
- CNES
- Google
- Site institucional
- LinkedIn
- Compras públicas
- Indicação
- Base interna
- Evento
- Outro

**Regra:**
- Todo lead precisa ter fonte.
- Sem fonte registrada, o lead não pode ser marcado como “Pronto para C2”.

---

### Link da fonte

**Tipo de campo:** URL desejável

**Exemplo:**
```text
https://cnes.datasus.gov.br/
```

**Regra:**
- Sempre preencher quando a fonte for online.
- Em caso de indicação verbal, deixar em branco e registrar a origem em “Observações C1”.

---

### Data de captura

**Tipo de campo:** Data obrigatória

**Regra:**
- Usar a data em que o lead foi inserido no CRM.
- Esse campo ajuda a medir frescor da base.

---

### Responsável pela captura

**Tipo de campo:** Pessoa obrigatório

**Regra:**
- Registrar quem incluiu o lead.
- Garante rastreabilidade e controle de qualidade.

---

## 4. Bloco C — Dados Complementares

Estes campos ajudam o C2, mas não devem travar o C1.

### CNES

**Tipo de campo:** Texto opcional

**Quando preencher:**
- Quando a instituição for encontrada no CNES/DATASUS.

**Uso:**
- Validação oficial.
- Deduplicação.
- Consulta posterior.

---

### CNPJ

**Tipo de campo:** Texto opcional

**Uso:**
- Desambiguação.
- Validação.
- Deduplicação.

---

### Site

**Tipo de campo:** URL opcional

**Uso:**
- Apoiar enriquecimento no C2.
- Facilitar contato no C3.

---

### Telefone geral

**Tipo de campo:** Telefone opcional

**Uso:**
- Acesso inicial.
- Não precisa ser contato direto.

**Regra:**
- Telefone geral é suficiente no C1.
- Não buscar telefone direto por mais de 3 minutos.

---

## 5. Bloco D — Sinais Iniciais

### Indícios relevantes

**Tipo de campo:** Texto curto

**Objetivo:** registrar sinais úteis para priorização inicial.

**Exemplos:**
```text
Hospital com UTI.
OS com múltiplas unidades.
Rede hospitalar privada.
Instituição encontrada em compra pública.
```

**Regra:**
- Usar frases curtas.
- Não escrever opinião subjetiva.
- Evitar “parece bom”, “alto potencial” ou “acho interessante”.

---

### Prioridade inicial C1

**Tipo de campo:** Seleção obrigatória

**Opções:**
- Alta
- Média
- Baixa
- Revisar

**Critérios:**

| Prioridade | Quando usar |
|---|---|
| Alta | OS, rede, hospital grande, hospital com UTI |
| Média | hospital médio ou instituição estruturada |
| Baixa | clínica pequena, home care limitado ou estrutura simples |
| Revisar | dados insuficientes ou dúvida relevante |

**Regra:**
- Essa prioridade não substitui o score do C2.
- Serve apenas para ordenar a fila de triagem.

---

## 6. Bloco E — Controle de Qualidade

### Duplicado?

**Tipo de campo:** Checkbox

**Quando marcar:**
- Existe registro igual ou muito parecido no CRM.

**Critérios de duplicidade:**
- Mesmo nome e município.
- Mesmo CNPJ.
- Mesmo CNES.
- Mesmo site.
- Mesmo telefone geral.
- Nome fantasia diferente, mas mesma instituição.

---

### Status C1

**Tipo de campo:** Seleção obrigatória

**Opções:**
- Novo
- Incompleto
- Pronto para C2
- Duplicado
- Fora do ICP
- Revisar depois

**Critérios:**

| Status | Quando usar |
|---|---|
| Novo | lead recém-capturado, ainda sem validação |
| Incompleto | faltam dados obrigatórios |
| Pronto para C2 | dados mínimos completos + fonte registrada |
| Duplicado | já existe no CRM |
| Fora do ICP | claramente irrelevante para a Santa Luzia |
| Revisar depois | dúvida que exige mais pesquisa |

---

### Data da última validação

**Tipo de campo:** Data opcional

**Uso:**
- Controlar atualização da base.
- Revisar dados antigos.

---

### Próxima etapa

**Tipo de campo:** Seleção

**Opções:**
- C2 — Triagem e Qualificação
- Revisar C1
- Arquivar
- Unificar duplicado

**Regra:**
- Se Status C1 = Pronto para C2 → Próxima etapa = C2.
- Se Status C1 = Duplicado → Próxima etapa = Unificar duplicado.
- Se Status C1 = Fora do ICP → Próxima etapa = Arquivar.
- Se Status C1 = Incompleto ou Revisar depois → Próxima etapa = Revisar C1.

---

## 7. Bloco F — Observações

### Observações C1

**Tipo de campo:** Texto

**Objetivo:** registrar contexto curto para ajudar C2.

**Modelo recomendado:**
```text
Fonte:
Contexto:
Dúvida:
Próxima ação:
```

**Exemplo:**
```text
Fonte: Google
Contexto: hospital localizado em Belém/PA, com site ativo.
Dúvida: confirmar se possui UTI.
Próxima ação: validar porte e fit no C2.
```

**Regra:**
- Não usar opiniões vagas.
- Não transformar observação em pesquisa longa.
- Texto deve ser útil para quem fará o C2.

---

## 8. Campos obrigatórios para enviar ao C2

O lead só pode ir para C2 se os campos abaixo estiverem preenchidos:

- Nome da instituição
- Tipo presumido
- Município
- UF
- Fonte do lead
- Data de captura
- Responsável pela captura
- Status C1 = Pronto para C2

---

## 9. Campos opcionais que agregam valor

- CNES
- CNPJ
- Site
- Telefone geral
- Link da fonte
- Indícios relevantes
- Observações C1

Esses campos melhoram a qualidade do C2, mas não são obrigatórios para encerrar o C1.

---

## 10. Regras automáticas recomendadas no CRM

### Regra 1 — Pronto para C2

Se:

```text
Nome da instituição preenchido
+ Tipo presumido preenchido
+ Município preenchido
+ UF preenchida
+ Fonte preenchida
+ Data de captura preenchida
+ Responsável preenchido
+ Não duplicado
```

Então:

```text
Status C1 = Pronto para C2
Próxima etapa = C2 — Triagem e Qualificação
```

---

### Regra 2 — Incompleto

Se faltar qualquer campo obrigatório:

```text
Status C1 = Incompleto
Próxima etapa = Revisar C1
```

---

### Regra 3 — Duplicado

Se checkbox “Duplicado?” estiver marcado:

```text
Status C1 = Duplicado
Próxima etapa = Unificar duplicado
```

---

### Regra 4 — Fora do ICP

Se a instituição for claramente irrelevante:

```text
Status C1 = Fora do ICP
Próxima etapa = Arquivar
```

---

## 11. Template visual do formulário

```text
# C1 — Captura de Lead

## Identificação
Nome da instituição:
Tipo presumido:
Município:
UF:

## Origem
Fonte do lead:
Link da fonte:
Data de captura:
Responsável:

## Dados complementares
CNES:
CNPJ:
Site:
Telefone geral:

## Sinais iniciais
Indícios relevantes:
Prioridade inicial C1:

## Controle
Duplicado?
Status C1:
Data da última validação:
Próxima etapa:

## Observações
Fonte:
Contexto:
Dúvida:
Próxima ação:
```

---

## 12. Exemplo preenchido

```text
# C1 — Captura de Lead

## Identificação
Nome da instituição: Hospital Exemplo Norte
Tipo presumido: Hospital
Município: Belém
UF: PA

## Origem
Fonte do lead: CNES
Link da fonte: https://cnes.datasus.gov.br/
Data de captura: 29/04/2026
Responsável: Maria

## Dados complementares
CNES: 1234567
CNPJ:
Site: https://www.hospitalexemplo.com.br
Telefone geral: (91) 0000-0000

## Sinais iniciais
Indícios relevantes: hospital geral com indício de UTI.
Prioridade inicial C1: Alta

## Controle
Duplicado? Não
Status C1: Pronto para C2
Data da última validação: 29/04/2026
Próxima etapa: C2 — Triagem e Qualificação

## Observações
Fonte: CNES + site institucional
Contexto: instituição hospitalar estruturada em Belém/PA.
Dúvida: confirmar número de leitos no C2.
Próxima ação: aplicar score de qualificação no C2.
```

---

## 13. Erros que o formulário evita

- Lead sem fonte.
- Lead sem cidade ou UF.
- Cadastro duplicado.
- Contato solto sem instituição.
- Envio prematuro para C2.
- Pesquisa excessiva no C1.
- Perda de conta estratégica por falta de contato direto.
- Observações subjetivas sem utilidade operacional.

---

## 14. Resultado esperado

Ao usar este formulário, o C1 passa a entregar para o C2 uma base:

- limpa;
- rastreável;
- padronizada;
- deduplicada;
- organizada por instituição;
- pronta para qualificação objetiva.

---

## 15. Resumo executivo

```text
O formulário C1 existe para garantir que toda instituição capturada entre no CRM com dados mínimos, fonte confiável e status claro.

Ele não qualifica profundamente.
Ele não vende.
Ele não exige contato direto.

Ele prepara o lead para o C2.
```
