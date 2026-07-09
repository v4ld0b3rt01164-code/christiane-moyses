# Prompt — Construção do site (Agente de codificação + Impeccable)

Cole este prompt no seu agente de codificação (com a skill/comandos Impeccable
disponíveis), dentro da pasta do projeto — com `PRODUCT-christiane-moyses.md`
(renomeado para `PRODUCT.md` na raiz do projeto) e `med-christiane-moyses.json`
já presentes.

---

Estou construindo o site institucional da Dra. Christiane Moysés (Cardiologia e
Clínica Médica, Miguelópolis-SP), a ser publicado no Cloudflare Pages. Já tenho dois
arquivos de contexto na raiz do projeto: `PRODUCT.md` (estratégia de marca) e
`med-christiane-moyses.json` (dados extraídos do Google Maps). Leia os dois antes de
começar.

Siga este fluxo, nesta ordem, sem pular etapas (comandos da skill Impeccable):

1. **`/impeccable init`** — se ainda não houver `PRODUCT.md`/`DESIGN.md`
   reconhecidos pela skill, rode para gerar a estrutura. Use o `PRODUCT.md` que já
   forneci como base real — não substitua o conteúdo, só complemente se necessário.
2. **`/impeccable shape`** — produza um brief de design a partir do `PRODUCT.md` e
   do JSON. Use os dados reais (nome, endereço, telefone, avaliações do Google). Os
   campos marcados `"A CONFIRMAR COM A CLIENTE"` devem virar placeholders visíveis e
   claramente sinalizados no brief — **não invente** conteúdo para esses campos.
3. **`/impeccable craft`** — desenhe e construa a primeira versão do site a partir
   do brief.
4. Depois que a primeira versão estiver construída: **`/impeccable document`** —
   gere o `DESIGN.md` real a partir do que foi implementado (não antes disso).
5. **`/impeccable critique`** seguido de **`/impeccable polish`** — revise e refine.
6. **`/impeccable audit`** — cheque problemas técnicos (estados de erro, i18n/PT-BR,
   responsividade, performance) antes de publicar.

## Requisitos técnicos

- Stack compatível com deploy estático no **Cloudflare Pages**.
- Registro: **brand surface** (site institucional, não app de produto) — ver
  `PRODUCT.md`.
- **Página única**, objetiva, **mobile-first**.
- Tom **sério e técnico, mas humano** — sem gatilhos de medo/urgência sobre saúde do
  coração — ver seção de voz no `PRODUCT.md`.
- CTA principal sempre visível: **WhatsApp/telefone** (`+55 16 98999-1790`).
- **Não inventar** textos institucionais genéricos, estatísticas ou depoimentos além
  dos fornecidos no JSON.
- **Não usar** fotos de banco de imagens genéricas de medicina (jaleco branco com
  prancheta, ícone de ECG genérico) — deixar placeholder de imagem real.
- Seguir as anti-referências listadas no `PRODUCT.md`.

## Dados da cliente

Ver `med-christiane-moyses.json` na raiz do projeto.
