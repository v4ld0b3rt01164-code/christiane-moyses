---
name: Dra. Christiane Moysés — Cardiologia e Clínica Médica
description: Site institucional de página única para médica cardiologista em Miguelópolis-SP
colors:
  pure-white: "oklch(1.000 0.000 0)"
  warm-surface: "oklch(0.965 0.005 25)"
  deep-ink: "oklch(0.180 0.010 20)"
  soft-ink: "oklch(0.450 0.005 20)"
  burgundy: "oklch(0.380 0.170 22)"
  burgundy-deep: "oklch(0.340 0.160 22)"
  burgundy-dark: "oklch(0.220 0.075 22)"
  burgundy-pale: "oklch(0.930 0.022 22)"
  muted: "oklch(0.550 0.005 20)"
  subtle-border: "oklch(0.880 0.005 20)"
  whatsapp-green: "oklch(0.540 0.185 155)"
typography:
  display:
    fontFamily: "Source Serif 4, Georgia, Times New Roman, serif"
    fontSize: "clamp(2.25rem, 1.6rem + 2.8vw, 3.75rem)"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Source Sans 3, system-ui, -apple-system, sans-serif"
    fontSize: "clamp(1rem, 0.95rem + 0.25vw, 1.0625rem)"
    fontWeight: 350
    lineHeight: 1.65
  label:
    fontFamily: "Source Sans 3, system-ui, -apple-system, sans-serif"
    fontSize: "clamp(0.75rem, 0.72rem + 0.15vw, 0.8125rem)"
    fontWeight: 600
    letterSpacing: "0.08em"
    textTransform: "uppercase"
rounded:
  sm: "4px"
  md: "8px"
  lg: "12px"
spacing:
  xs: "clamp(0.25rem, 0.2rem + 0.25vw, 0.5rem)"
  sm: "clamp(0.5rem, 0.4rem + 0.5vw, 0.75rem)"
  md: "clamp(0.75rem, 0.6rem + 0.75vw, 1.25rem)"
  lg: "clamp(1.25rem, 1rem + 1.25vw, 2.5rem)"
  xl: "clamp(2rem, 1.5rem + 2.5vw, 4rem)"
  2xl: "clamp(3rem, 2rem + 4vw, 6rem)"
components:
  button-primary:
    backgroundColor: "{colors.burgundy}"
    textColor: "{colors.pure-white}"
    rounded: "{rounded.md}"
    padding: "0.75em 1.5em"
  button-primary-hover:
    backgroundColor: "{colors.burgundy-deep}"
  button-whatsapp:
    backgroundColor: "{colors.whatsapp-green}"
    textColor: "{colors.pure-white}"
    rounded: "{rounded.md}"
    padding: "0.75em 1.5em"
  button-light:
    backgroundColor: "{colors.pure-white}"
    textColor: "{colors.burgundy}"
    rounded: "{rounded.md}"
    padding: "0.85em 2em"
---

# Design System: Dra. Christiane Moysés

## 1. Overview

**Creative North Star: "O Consultório ao Entardecer"**

Um consultório médico em cidade pequena ao entardecer — luz quente filtrada por persianas, madeira escura, confiança silenciosa. O sistema visual traduz a seriedade técnica da cardiologia com o acolhimento da clínica médica geral. Não é um hospital frio, não é um app de telemedicina corporativo: é o consultório da médica de confiança da família.

A paleta gira em torno de um bordô profundo extraído do logotipo da marca, ancorando seções escuras que contrastam com superfícies brancas puras. A tipografia combina uma serifa humanista quente (Source Serif 4) para autoridade nas headings com uma sans limpa e técnica (Source Sans 3) para legibilidade no corpo. O layout é de página única, mobile-first, com ritmo variado entre seções claras e escuras.

O sistema rejeita explicitamente: ícones de ECG genéricos, fotos stock de jaleco branco, glassmorphism, gradientes roxos, texto vazio estilo "cuidando da sua saúde com excelência", e qualquer tom de urgência ou medo sobre saúde cardíaca.

**Key Characteristics:**
- Committed color strategy: o bordô carrega 30-60% da superfície
- Serif display + sans body em contraste de estrutura
- Escala fluid com clamp() em tipografia e espaçamento
- Sombras sutis, sem exagero de profundidade
- Seções alternadas claro/escuras para ritmo visual
- CTA de WhatsApp sempre visível (header fixo + botão flutuante)

## 2. Colors

A paleta é intencionalmente contida em número de cores, mas comprometida em intensidade. O bordô da marca domina; o branco puro garante assepsia visual médica.

### Primary
- **Burgundy** (oklch(0.380 0.170 22)): Cor âncora da marca, extraída do logotipo. Usada em botões principais, headings em seções claras, e como cor de destaque. Botões com texto branco puro.
- **Burgundy Deep** (oklch(0.340 0.160 22)): Hover state do primary. Escurecimento sutil que mantém a saturação.
- **Burgundy Dark** (oklch(0.220 0.075 22)): Fundo de seções escuras (Sobre, Contato). Texto branco sobre esta cor. Transmite profundidade sem pesar.
- **Burgundy Pale** (oklch(0.930 0.022 22)): Fundo de hover para botões outline. Tonalidade quase branca com um sopro de bordô.

### Secondary
- **WhatsApp Green** (oklch(0.540 0.185 155)): Usado exclusivamente nos botões de WhatsApp. Cor de ação, não de marca. Distinta do bordô para reconhecimento imediato da plataforma.

### Neutral
- **Pure White** (oklch(1.000 0.000 0)): Fundo principal. Branco absoluto, sem tintura escondida. A "assepsia" visual que o contexto médico pede.
- **Warm Surface** (oklch(0.965 0.005 25)): Fundo alternativo para seções (Serviços). Levemente tintado em direção ao bordô para coesão, mas imperceptível como cor.
- **Deep Ink** (oklch(0.180 0.010 20)): Texto corpo. Contraste ≥7:1 sobre branco. Leve crominância para não ser cinza puro.
- **Soft Ink** (oklch(0.450 0.005 20)): Texto secundário, metadados, labels. Contraste ≥4.5:1.
- **Muted** (oklch(0.550 0.005 20)): Texto terciário, footer. Uso mínimo.
- **Subtle Border** (oklch(0.880 0.005 20)): Bordas de cards, separadores.

### Named Rules
**The Committed Rule.** O bordô não é um acento tímido de 10%. Ele carrega 30-60% da superfície total da página — seja como fundo de seções inteiras, seja como cor de headings e botões. Sua presença é a voz da marca.

**The White-Is-White Rule.** O fundo principal é branco puro (oklch(1 0 0)), não "off-white", não "cream", não "paper". A assepsia é intencional. O calor da marca vem do bordô e da tipografia, não do fundo.

## 3. Typography

**Display Font:** Source Serif 4 (com fallback Georgia, Times New Roman, serif)
**Body Font:** Source Sans 3 (com fallback system-ui, -apple-system, sans-serif)

**Character:** Uma serifa humanista quente para autoridade médica encontra uma sans limpa e técnica para legibilidade. O contraste está no eixo serif/sans, não em peso ou escala. Ambas são da mesma fundição (Adobe Source), garantindo coesão de proporções.

### Hierarchy
- **Display** (500, clamp(2.25rem, 1.6rem + 2.8vw, 3.75rem), 1.15): Nome da médica no hero. Uso único, máxima hierarquia. letter-spacing: -0.02em.
- **Headline** (500, clamp(1.75rem, 1.4rem + 1.5vw, 2.5rem), 1.15): Títulos de seção (h2). text-wrap: balance.
- **Title** (500, clamp(1.375rem, 1.2rem + 0.8vw, 1.75rem), 1.15): Subtítulos (h3).
- **Body** (350, clamp(1rem, 0.95rem + 0.25vw, 1.0625rem), 1.65): Texto corrido. max-width: 65ch. text-wrap: pretty. Peso 350 (mais leve que o padrão 400) para leitura confortável na sans.
- **Label** (600, clamp(0.75rem, 0.72rem + 0.15vw, 0.8125rem), 1.4, 0.08em, uppercase): Labels de contato e badges. Uso restrito — não como "eyebrow" em todas as seções.

### Named Rules
**The Single Eyebrow Rule.** Labels uppercase com tracking existem em exatamente um lugar: o badge "A CONFIRMAR COM A CLIENTE" na seção Sobre. Nenhuma outra seção repete o padrão. Um kicker é voz; repeti-lo em todas as seções é gramática de IA.

**The Body-Light Rule.** O texto corpo usa peso 350 (Source Sans 3 "Light"), não 400. A sans em peso mais leve respira melhor em português e compensa a densidade da informação médica.

## 4. Elevation

Sistema majoritariamente plano com elevação sutil em pontos de destaque. A profundidade é comunicada por cor (seções escuras vs claras), não por sombra. Sombras aparecem apenas como resposta a estado ou para destacar elementos isolados.

### Shadow Vocabulary
- **Ambient Low** (0 1px 2px oklch(0 0 0 / 0.06)): Cards em grid de serviços no hover.
- **Ambient Mid** (0 4px 12px oklch(0 0 0 / 0.08)): Card de avaliações.
- **Ambient High** (0 8px 30px oklch(0 0 0 / 0.10)): Imagem na seção Sobre.
- **WhatsApp Glow** (0 4px 20px oklch(0.540 0.150 155 / 0.40)): Botão flutuante de WhatsApp. A sombra é tintada de verde para reforçar a identidade da plataforma.

### Named Rules
**The Flat-By-Default Rule.** Superfícies são planas em repouso. Sombras aparecem apenas em hover ou para isolar elementos de destaque (card de reviews, imagem). Nenhuma seção tem sombra decorativa.

## 5. Components

### Buttons
- **Shape:** Bordas arredondadas sutis (8px). Cantos vivos passam frieza hospitalar; cantos muito redondos passam informalidade. 8px é o equilíbrio médico.
- **Primary (Burgundy):** Fundo bordô, texto branco puro. Padding fluido (0.75em 1.5em). Hover escurece para burgundy-deep. Transição de 0.2s ease em background-color. Altura mínima 44px (touch target).
- **WhatsApp:** Fundo verde WhatsApp, texto branco. Usado no header, hero CTA e botão flutuante fixo. Ícone de WhatsApp inline SVG.
- **Light (on dark):** Fundo branco, texto bordô. Usado exclusivamente sobre seções escuras (Contato). Hover: branco levemente escurecido.
- **Outline:** Borda 1.5px na cor currentColor, fundo transparente. Hover preenche com burgundy-pale. Uso secundário.

### Cards / Containers
- **Service Item:** Fundo branco, borda sutil (1px subtle-border), raio 8px. Padding interno fluido (--space-md). Ícone check-circle inline SVG + nome do serviço. Hover: borda muda para burgundy, sombra ambient-low.
- **Review Card:** Fundo branco, borda 1px, raio 12px. Padding generoso (--space-xl). Sombra ambient-mid. Layout vertical centrado: estrelas → pontuação → contagem → citação → fonte.
- **Contact Item:** Fundo com 6% de branco sobre burgundy-dark, borda com 10% de branco. Raio 8px. Link completo (clickável). Hover: fundo sobe para 10% de branco.
- **About Placeholder:** Fundo com 8% de branco sobre burgundy-dark, borda dashed com 20% de branco. Raio 12px. Padding generoso. Badge "A CONFIRMAR" com ícone de alerta.

### Navigation
- **Header:** Sticky no topo (z-index 100). Fundo branco com 92% de opacidade + backdrop-filter blur(12px). Borda inferior sutil. Logo à esquerda, botão WhatsApp à direita. Altura 3.5rem. No mobile, mantém os mesmos elementos sem colapsar.

### Fixed CTA
- **WhatsApp Float:** Posição fixed no canto inferior direito. Fundo verde WhatsApp, borderRadius 999px (pill). Sombra com glow verde. Padding 0.75em 1.25em. No mobile (<480px), mostra apenas ícone; acima disso, ícone + texto "WhatsApp". Hover: translateY(-2px) + sombra expandida.

## 6. Do's and Don'ts

### Do:
- **Do** usar o bordô como cor dominante — ele carrega 30-60% da superfície da página
- **Do** usar branco puro (oklch(1 0 0)) como fundo principal, sem tintura
- **Do** manter o WhatsApp sempre visível (header + botão flutuante + seção de contato)
- **Do** usar texto real e verificável — nome, CRM 141228, serviços confirmados, avaliação do Google
- **Do** sinalizar conteúdo pendente com o badge "A CONFIRMAR COM A CLIENTE"
- **Do** usar as imagens reais do projeto (logo, equipamentos), não stock photos
- **Do** manter tom sério e técnico, mas humano — informar com serenidade, não com susto
- **Do** respeitar mobile-first: tudo funciona em 320px de largura
- **Do** usar inline SVGs para ícones, sem dependência de bibliotecas externas

### Don't:
- **Don't** usar ícone de coração com batimento (ECG line) genérico
- **Don't** usar stock photo de médico de jaleco sorrindo com prancheta
- **Don't** usar gradientes roxo/glassmorphism, padrão "gerado por IA"
- **Don't** escrever textos vazios tipo "cuidando da sua saúde com excelência e dedicação" sem informação concreta
- **Don't** soar como app de telemedicina corporativo — é uma médica local, não uma plataforma de saúde digital
- **Don't** usar tom de urgência/alarme (ex: "não ignore os sinais do seu coração!!")
- **Don't** inventar estatísticas, depoimentos ou formações não confirmadas pela cliente
- **Don't** usar azul/verde "hospitalar" frio e distante
- **Don't** usar side-stripe borders (border-left/right > 1px como acento colorido)
- **Don't** usar gradient text (background-clip: text com gradiente)
- **Don't** usar cards aninhados
- **Don't** repetir eyebrow labels uppercase em todas as seções
- **Don't** usar mais de 2 font families
- **Don't** colocar cinza sobre fundo colorido — usar transparência do branco ou tom mais escuro da mesma hue
