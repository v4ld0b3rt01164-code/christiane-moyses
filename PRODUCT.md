# PRODUCT.md — Site institucional: Dra. Christiane Moysés Cardiologia e Clínica Médica

> Arquivo de estratégia para a skill Impeccable. Ler antes de qualquer comando de design.

## Quem é a cliente

Médica atuando em Cardiologia e Clínica Médica em Miguelópolis-SP. Reputação local muito
forte (5.0★, 26 avaliações — o maior volume entre os médicos levantados na cidade). Hoje
só existe online via perfis em diretórios médicos (Doctoralia, Médicos Brasil), sem site
próprio.

- **CRM:** 141228 (confirmado via arte publicada pela médica no Google Maps)
- **A CONFIRMAR COM A CLIENTE:** formação acadêmica, tempo de atuação, se atende convênios.

## Audiência

- Moradores de Miguelópolis e região, com foco em pacientes de meia-idade/idosos que
  buscam acompanhamento cardiológico contínuo, além de clínica médica geral para a
  família.
- Público que valoriza seriedade médica e continuidade de cuidado — não é uma decisão
  por impulso, é uma escolha de longo prazo de "meu médico de confiança".
- Muitos vindo de indicação; acesso majoritariamente via celular.

## Propósito do site

Reforçar credibilidade médica e facilitar o agendamento. O visitante precisa perceber
seriedade profissional e clareza sobre especialidades atendidas (coração + clínica geral),
saindo com confiança suficiente para agendar consulta. CTA principal: telefone/WhatsApp.

## Voz de marca / tom

- **Sério e técnico, mas humano** — a especialidade (cardiologia) exige transmitir
  competência e precisão; ao mesmo tempo, clínica médica geral pede acolhimento.
- Evitar tom de urgência/alarme (não usar medo como gatilho, ex: "não ignore os sinais
  do seu coração!!") — informar com serenidade, não com susto.
- Linguagem clara sobre quando procurar cardiologista vs. clínico geral, sem jargão
  médico não explicado.

## Registro

**Brand surface** — site institucional de confiança médica, não app de produto.

## Anti-referências

- Clichês de clínica: ícone de coração com batimento (ECG line) genérico, stock photo
  de médico de jaleco sorrindo com prancheta, azul/verde "hospitalar" frio e distante.
- Gradientes roxo/glassmorphism, padrão "gerado por IA".
- Textos vazios tipo "cuidando da sua saúde com excelência e dedicação" sem informação
  concreta sobre especialidades ou abordagem.
- Nada que soe como app de telemedicina corporativo — é uma médica local, não uma
  plataforma de saúde digital.

## Conteúdo já disponível (fonte: Google Maps + arte publicada pela médica)

- Nome: Dra. Christiane Moysés - Cardiologia e Clínica Médica
- CRM: 141228
- Endereço: Av. José Espírito Santo Tanajura, 14 - Centro, Miguelópolis - SP
- Telefone/WhatsApp: +55 16 98999-1790
- Instagram: @Chrismoyses
- Avaliação Google: 5.0★ (26 avaliações)
- Serviços: Cardiologia Geral, Arritmias, Cardiologia Geriátrica, Cardiopatias,
  Eletrocardiograma, Hipertensão Arterial, Insuficiência Cardíaca / Angina,
  Dislipidemias, Infarto do Miocárdio, Holter 24h, MAPA 24h, Coronariopatias

## Pendências antes do design final (A CONFIRMAR COM A CLIENTE)

- [x] CRM (141228 — confirmado via arte publicada no Google Maps)
- [x] Exames/procedimentos realizados no local (lista de 12 serviços confirmada)
- [x] Instagram (@Chrismoyses)
- [x] Foto profissional (foto-dra.png fornecida pela cliente)
- [ ] Formação acadêmica e especialização
- [ ] Texto "sobre" (tempo de atuação, abordagem com pacientes)
- [ ] Horário de funcionamento e convênios atendidos
- [ ] E-mail de contato
- [ ] Autorização para publicar nome, avaliações e dados no site

## Infraestrutura de publicação

- Hospedagem/CDN: Cloudflare Pages (https://christiane-moyses.pages.dev)
- Stack: Astro (static site generator, output estático)
- Deploy: wrangler pages deploy (manual) + GitHub Actions (Workflow pendente de scope)
- Repositório: https://github.com/v4ld0b3rt01164-code/christiane-moyses

## Assets do projeto

| Arquivo | Tipo | Uso no site |
|---------|------|-------------|
| `logo-color.png` | Logo | Favicon no Layout.astro |
| `foto-dra.png` | Foto | Seção Sobre (split-panel direito) |
| `cardio- (1).png` | Imagem | Hero visual (coração 3D, split-panel direito) |
| `cardio- (1).jpg` | Imagem | Seção Serviços (split-panel esquerdo) + textura ::before |
| `ecg_transparent.png` | PNG | Animação ECG no hero (acima do h1, sweep-reveal JS) |
| `atuacao.jpg` | Imagem | Seção Serviços (split-panel esquerdo, áreas de atuação) |
| `pulse.svg` | SVG | Ícone de pulso no header NAV |
