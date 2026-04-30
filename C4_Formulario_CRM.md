
# FORMULÁRIO CRM — C4 VISITA TÉCNICA COMERCIAL

## 1. Identificação da Oportunidade

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Nome do cliente/paciente | Texto | Sim | |
| Tipo de cliente | Lista | Sim | Familiar / Home Care / Hospital / Clínica / Nutricionista / Outro |
| Origem do lead | Lista | Sim | Indicação / Hospital / WhatsApp / Instagram / Outro |
| Telefone principal | Texto | Sim | |
| Cidade/Bairro | Texto | Sim | |
| Responsável pelo contato | Texto | Sim | |
| Responsável pela decisão | Texto | Sim | |
| Responsável pelo pagamento | Texto | Sim | |

---

## 2. Prescrição e Necessidade

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Prescrição recebida | Sim/Não/Parcial | Sim | |
| Prescrição legível | Sim/Não | Condicional | |
| Foto da prescrição | Upload | Recomendado | |
| Produto solicitado | Texto | Sim | |
| Produto validado | Texto | Sim | |
| Quem indicou | Texto | Não | |
| Já usa atualmente? | Sim/Não | Não | |
| Produto atual | Texto | Não | |
| Urgência | Lista | Sim | Imediato / 24h / 48h / Sem urgência |

---

## 3. Consumo e Volume

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Quantidade por dia | Número | Condicional | |
| Frequência de uso | Lista | Condicional | Diário / Intermitente |
| Quantidade mensal estimada | Número | Sim | |
| Tipo de demanda | Lista | Sim | Pontual / Recorrente / Indefinido |
| Frequência de recompra | Texto | Não | |

---

## 4. Logística e Entrega

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Endereço completo | Texto | Sim | |
| Ponto de referência | Texto | Não | |
| Restrição de entrega | Sim/Não | Não | |
| Descrição da restrição | Texto | Não | |
| Quem recebe | Texto | Sim | |
| Horário de entrega | Texto | Não | |
| Precisa entrega recorrente | Sim/Não | Sim | |
| Observação de armazenamento | Texto | Não | |

---

## 5. Comercial

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Forma de pagamento provável | Lista | Sim | Pix / Cartão / Faturado / Outro |
| Precisa de orçamento formal | Sim/Não | Sim | |
| Sensibilidade a preço | Lista | Não | Baixa / Média / Alta |
| Existe concorrente | Sim/Não | Não | |
| Já comprou da empresa | Sim/Não | Não | |
| Exige documento específico | Sim/Não | Não | |

---

## 6. Riscos

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Risco técnico | Sim/Não | Não | |
| Risco logístico | Sim/Não | Não | |
| Risco comercial | Sim/Não | Não | |
| Descrição do risco | Texto | Não | |

---

## 7. Classificação da C4

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Saída da C4 | Lista | Sim | Proposta / Venda direta / Recorrência / Pendente / Desqualificado |
| Motivo (se aplicável) | Texto | Condicional | |
| Tipo de venda final | Lista | Sim | Pontual / Recorrente |
| Próximo passo | Texto | Sim | |
| Responsável pelo próximo passo | Texto | Sim | |
| Data de follow-up | Data | Sim | |

---

## 8. Evidências

| Campo | Tipo | Obrigatório | Observação |
|------|------|------------|-----------|
| Foto da prescrição | Upload | Não | |
| Fotos adicionais | Upload | Não | |
| Documentos anexos | Upload | Não | |

---

## Regras de Uso

- Não avançar para C5 sem: produto validado, quantidade mensal, pagador, endereço e saída da C4.
- Toda C4 deve ter próximo passo e data de follow-up.
- Se recorrente, definir frequência obrigatoriamente.
- Não realizar orientação clínica fora do escopo comercial.
