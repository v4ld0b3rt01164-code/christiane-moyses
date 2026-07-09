---
name: Dra. Christiane Moysés — Cardiologia e Clínica Médica
description: Site institucional de página única para médica cardiologista em Miguelópolis-SP
colors:
  ruby: "#C2181C"
  mahogany: "#5C2D2A"
  warm-sand: "#C7A48D"
  office-cream: "#E8E2D9"
  pure-white: "#FFFFFF"
  soft-ink: "#1E1817"
typography:
  display:
    fontFamily: "Work Sans, system-ui, -apple-system, sans-serif"
    fontSize: "clamp(2.25rem, 1.6rem + 2.8vw, 3.5rem)"
    fontWeight: 700
    lineHeight: 1.12
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Work Sans, system-ui, -apple-system, sans-serif"
    fontSize: "clamp(1rem, 0.95rem + 0.25vw, 1.0625rem)"
    fontWeight: 350
    lineHeight: 1.65
  label:
    fontFamily: "Work Sans, system-ui, -apple-system, sans-serif"
    fontSize: "clamp(0.75rem, 0.72rem + 0.15vw, 0.8125rem)"
    fontWeight: 600
    letterSpacing: "0.08em"
    textTransform: "uppercase"
rounded:
  sm: "4px"
  md: "8px"
  lg: "12px"
  pill: "999px"
spacing:
  xs: "clamp(0.25rem, 0.2rem + 0.25vw, 0.5rem)"
  sm: "clamp(0.5rem, 0.4rem + 0.5vw, 0.75rem)"
  md: "clamp(0.75rem, 0.6rem + 0.75vw, 1.25rem)"
  lg: "clamp(1.25rem, 1rem + 1.25vw, 2.5rem)"
  xl: "clamp(2rem, 1.5rem + 2.5vw, 4rem)"
  2xl: "clamp(3rem, 2rem + 4vw, 6rem)"
components:
  button-primary:
    backgroundColor: "{colors.ruby}"
    textColor: "{colors.pure-white}"
    rounded: "{rounded.md}"
    padding: "0.75em 1.5em"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.ruby}"
    border: "1.5px solid {colors.ruby}"
    rounded: "{rounded.md}"
  dock-whatsapp:
    backgroundColor: "{colors.ruby}"
    textColor: "{colors.pure-white}"
    rounded: "{rounded.md}"
  dock-phone:
    backgroundColor: "transparent"
    textColor: "{colors.ruby}"
    border: "1.5px solid {colors.ruby}"
    rounded: "{rounded.md}"
---

# Design System: Dra. Christiane Moysés

## 1. Overview

**Creative North Star: "O Consultório ao Entardecer"**

Sistema visual para site institucional de cardiologista em Miguelópolis-SP. Paleta derivada do `servicos.png` e `logo-color.png` da médica — ruby red do logo, mahogany do painel de serviços, office cream da parede do consultório. Single page, mobile-first, Astro static.

Tipografia única (Work Sans) ecoando o logo sans-serif. Split-panel como motivo estrutural extraído do `servicos.png`. ECG animado no hero referenciando o `eletro.svg`. Dock fixo mobile-only com WhatsApp + telefone.

**Key Characteristics:**
- Família tipográfica única (Work Sans 300-700)
- Paleta de 6 cores derivada dos assets originais
- Split-panel alternado claro/escuro
- ECG animado via CSS `stroke-dashoffset` no hero
- Dock fixo inferior apenas em mobile (<768px)
- Zero JavaScript — 100% HTML + CSS

## 2. Colors

Paleta extraída diretamente das imagens fornecidas pela médica.

### Primary
- **Ruby** (#C2181C): Cor do coração+ECG no `logo-color.png`. CTAs, dock WhatsApp, ECG animado.
- **Mahogany** (#5C2D2A): Fundo do painel escuro no `servicos.png`. Seções Serviços e Contato.
- **Warm Sand** (#C7A48D): Cor do nome no painel do `servicos.png`. Headings em seções escuras.
- **Office Cream** (#E8E2D9): Cor da parede no `servicos.png`. Fundo da seção Sobre.

### Neutral
- **Pure White** (#FFFFFF): Cor do texto no `logo-color.png`. Fundo principal.
- **Soft Ink** (#1E1817): Texto corpo. Derivado do marrom-escuro.

## 3. Typography

**Font:** Work Sans (com fallback system-ui, -apple-system, sans-serif)

Família única seguindo o logo 100% sans-serif. Contraste via peso (300-700), não via serif/sans.

### Hierarchy
- **Display** (700, clamp(2.25rem, 1.6rem + 2.8vw, 3.5rem), 1.12): h1 — nome da médica
- **Headline** (600, clamp(1.75rem, 1.4rem + 1.5vw, 2.5rem), 1.12): h2 — títulos de seção
- **Title** (500, clamp(1.375rem, 1.2rem + 0.8vw, 1.75rem), 1.12): h3 — subtítulos
- **Body** (350, clamp(1rem, 0.95rem + 0.25vw, 1.0625rem), 1.65): Texto corpo
- **Label** (600, clamp(0.75rem, 0.72rem + 0.15vw, 0.8125rem), uppercase): Labels e badges

## 4. Elevation

Sistema plano com sombras apenas em hover ou destaque. Profundidade comunicada por cor (seções claras vs escuras).

- **ambient-low**: 0 1px 3px — hover de service items
- **ambient-mid**: 0 4px 16px — card de reviews
- **ambient-high**: 0 8px 32px — imagens em split-media
- **ruby-glow**: 0 4px 24px rgba(194,24,28,0.30) — dock WhatsApp

### Named Rules
**The Flat-By-Default Rule.** Superfícies planas em repouso. Sombras apenas em hover/destaque.

## 5. Components

### Header
- Sticky, blur glass (92% opacidade + backdrop-filter). Altura 3.5rem.
- Esquerda: pulse.svg animado + "Christiane Moysés" | CARDIOLOGIA
- Sem logo — nome em texto puro.

### Hero
- Split-panel: texto (esquerda) + coração 3D (direita).
- ECG (`eletro.svg`) animado via CSS stroke-dashoffset acima do h1.
- Badges: CRM 141228 + Miguelópolis-SP.
- Sem estrelas ou CTA no hero — CTAs no dock mobile.

### Services
- Fundo mahogany com textura ECG (cardio- (1).jpg como ::before).
- Split-panel: imagem ECG paper (esquerda) + grid de 12 serviços (direita).
- Lista plana, sem agrupamento por categoria.

### About
- Fundo office cream. Split-panel: placeholder (esquerda) + foto-dra.png (direita).
- Badge "A CONFIRMAR COM A CLIENTE" com ícone de alerta.

### Reviews
- Card centralizado: 5.0 + 26 avaliações + citação.
- Divisor ECG decorativo entre heading e card.

### Contact
- Fundo mahogany. Grid 2×2: Telefone, WhatsApp, Endereço, Instagram.
- Itens clickáveis com hover state.

### Bottom Dock (mobile-only)
- Fixo na base. Dois botões: WhatsApp (ruby preenchido) + Ligar (outline ruby).
- safe-area-inset-bottom para iPhone.
- Oculto em ≥768px.

## 6. Do's and Don'ts

### Do:
- **Do** usar ruby #C2181C como cor de destaque (derivada do logo)
- **Do** usar mahogany #5C2D2A para seções escuras (derivado do servicos.png)
- **Do** manter WhatsApp e telefone sempre acessíveis via dock mobile
- **Do** usar Work Sans (família única, sans-serif, ecoando o logo)
- **Do** usar imagens reais fornecidas pela cliente
- **Do** sinalizar conteúdo pendente com badge "A CONFIRMAR COM A CLIENTE"
- **Do** manter tom sério e técnico, mas humano

### Don't:
- **Don't** usar Source Serif/Source Sans (substituído por Work Sans)
- **Don't** usar verde WhatsApp genérico no CTA (ruby da marca)
- **Don't** usar ícone de ECG genérico (o ECG do site é o eletro.svg da médica)
- **Don't** usar stock photos de jaleco/prancheta
- **Don't** usar glassmorphism, gradientes roxos, ou padrão "gerado por IA"
- **Don't** usar azul/verde hospitalar frio
- **Don't** usar tom de urgência/alarme sobre saúde cardíaca
- **Don't** inventar estatísticas ou depoimentos
