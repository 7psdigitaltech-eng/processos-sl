
# FORMULÁRIO CRM — C5 GESTÃO DE OBJEÇÕES

## 1. Identificação da Objeção

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Existe objeção | Sim/Não | Sim | |
| Data da objeção | Data | Sim | |
| Etapa onde surgiu | Lista | Sim | C3 / C4 / C5 / C6 / Pós-venda |

---

## 2. Descrição da Objeção

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Descrição da objeção (fala do cliente) | Texto longo | Sim | Registrar exatamente como o cliente falou |
| Contexto da objeção | Texto | Não | Situação em que surgiu |

---

## 3. Classificação

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Tipo de objeção | Lista | Sim | Preço / Fornecedor atual / Orçamento / Prescrição / Logística / Decisor / Confiança / Prazo / Contrato / Produto / Concorrência / Sem urgência |
| Origem da objeção | Lista | Sim | Falha C4 / Mercado / Cliente / Operacional |

---

## 4. Diagnóstico

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Causa provável | Texto | Sim | |
| Comparação mencionada | Texto | Não | Ex: fornecedor X |
| Quem decide | Texto | Não | |
| Falta algo para decisão? | Texto | Não | |

---

## 5. Tratamento

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Resposta aplicada | Texto | Sim | |
| Tipo de resposta | Lista | Sim | Argumento / Ajuste / Follow-up / Escalonamento |
| Houve desconto | Sim/Não | Sim | |
| Desconto aprovado | Sim/Não | Condicional | Se houve desconto |
| Necessitou escalonamento | Sim/Não | Sim | |

---

## 6. Encaminhamento

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Próximo passo | Texto | Sim | |
| Responsável | Texto | Sim | |
| Data de follow-up | Data | Sim | |
| Status da objeção | Lista | Sim | Aberta / Em tratamento / Resolvida / Perdida |

---

## 7. Resultado

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Objeção resolvida | Sim/Não | Sim | |
| Impacto na venda | Lista | Sim | Avançou / Travou / Perdeu |
| Motivo de perda | Texto | Condicional | Se perdeu |

---

## Regras de Uso

- Não avançar oportunidade sem definir próximo passo.
- Não dar desconto sem diagnóstico.
- Registrar toda objeção relevante no CRM.
- Máximo 2 tentativas sem evolução antes de reavaliar.
- Escalar objeções críticas (contrato, grande cliente, risco).

---

## Versão Mínima

Se simplificar:

- Tipo de objeção
- Descrição
- Próximo passo
- Follow-up
- Status

---

## Objetivo do Formulário

Padronizar a gestão de objeções, reduzir perda de informação, melhorar conversão e gerar aprendizado contínuo no processo comercial.
