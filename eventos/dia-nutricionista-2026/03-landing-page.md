# 03 — Landing page do evento

## 1. Objetivo

Criar uma landing page responsiva, elegante e de baixa fricção que funcione como extensão do convite recebido pelo WhatsApp.

A página tem três objetivos, nesta ordem:

1. **Encantar**
2. **Confirmar**
3. **Aproximar**

Não deve ser construída como catálogo ou página de vendas.

## 2. Acesso individualizado

### Recomendação

Cada convite deve receber um identificador único.

Exemplo conceitual:

```text
/evento/29-08?convite=8F72K
```

O identificador deve permitir que o sistema localize a convidada sem exigir que ela redigite informações já conhecidas pela Santa Luzia.

### Resultado esperado

Ao abrir a página, o sistema pode reconhecer a convidada e exibir uma saudação personalizada, por exemplo:

> Olá, Ana! Preparamos este momento especialmente para você.

### Regra de segurança

O identificador do convite não deve expor dados pessoais diretamente na URL. A implementação deve usar um token/identificador sem significado semântico e validar o vínculo no backend.

## 3. Estrutura recomendada da página

### Bloco 1 — Hero

Elementos:

- marca Santa Luzia;
- identidade visual do convite;
- “Save the Date”;
- data 29/08;
- “Jantar Comemorativo em Homenagem ao Dia do Nutricionista”;
- frase curta de posicionamento;
- CTA principal.

CTA:

**Confirmar minha presença**

### Bloco 2 — Uma noite especial

Apresentar os principais elementos da experiência:

- celebração;
- networking;
- jantar;
- apresentação das linhas Nutro e Pro Diet;
- valorização da profissão.

### Bloco 3 — Informações do evento

Quando definidos:

- data;
- horário;
- local;
- endereço;
- mapa/direções;
- estacionamento;
- dress code;
- outras orientações práticas.

### Bloco 4 — Confirmação

Título sugerido:

> Confirme sua presença

Texto de apoio:

> Será uma alegria receber você neste momento especial.

Campos recomendados:

- nome — preenchido quando possível;
- WhatsApp — preenchido quando possível;
- e-mail — somente se necessário para a operação;
- resposta de presença.

Ações:

- **Confirmar presença**
- **Não poderei comparecer**

### Bloco 5 — Confirmação concluída

Após confirmação, exibir uma experiência específica para quem confirmou.

Exemplo:

> Presença confirmada! ✨
>
> Estamos muito felizes em ter você conosco.

A página pode revelar conteúdos adicionais após a confirmação.

### Bloco 6 — Santa Luzia

Apresentação curta da distribuidora, coerente com o posicionamento institucional do site.

Mensagem-chave:

> A Santa Luzia atua na distribuição especializada em nutrição clínica, conectando profissionais e instituições a soluções para diferentes contextos de cuidado.

O texto final deve ser alinhado ao conteúdo institucional oficial da marca.

### Bloco 7 — Marcas parceiras

Apresentar **Nutro** e **Pro Diet** como parte do ecossistema que estará presente no evento.

Para cada marca:

- logo oficial;
- descrição curta;
- proposta de valor;
- 3 ou 4 soluções/produtos estratégicos, no máximo, quando fizer sentido;
- link opcional para conteúdo institucional/produtos.

### Bloco 8 — Encerramento

Reforçar o caráter de homenagem e relacionamento.

Exemplo de conceito:

> Um encontro para valorizar quem transforma a nutrição em cuidado e qualidade de vida.

CTA final:

**Contamos com você!**

## 4. Estado da página

A página deve apresentar conteúdos diferentes conforme o estado da convidada.

| Estado | Experiência |
|---|---|
| Convite sem resposta | CTA de confirmação |
| Confirmada | Confirmação + conteúdo pré-evento |
| Recusou | Mensagem de agradecimento + opção de contato futuro |
| Evento encerrado | Experiência pós-evento |

## 5. Requisitos de UX

- mobile first;
- carregamento rápido;
- botão de confirmação visível;
- formulário curto;
- boa leitura em WhatsApp browser;
- identidade visual consistente com o convite;
- acessibilidade básica de contraste e tamanho de fonte;
- nenhuma etapa desnecessária entre convite e confirmação.

## 6. Requisitos técnicos

A solução deve permitir:

- leitura do identificador individual;
- consulta da convidada;
- exibição do estado atual;
- gravação da confirmação/recusa;
- registro da data/hora da interação;
- integração com o CRM;
- disparo de eventos para automação;
- proteção contra submissões duplicadas.

## 7. Regra de negócio importante

Confirmar presença não deve criar outra pessoa/contato no CRM.

A ação deve atualizar a relação **contato/convidada ↔ evento**.

Isso evita retrabalho e duplicidade de cadastro.
