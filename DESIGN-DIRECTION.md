# Morgen — Direção de arte (Everton · Etapa 2)

**Status:** aprovado · base da Etapa 4  
**Pipeline:** static HTML/CSS/JS · branch `feat/media-mockup`  
**Dials:** variance **4** · motion **3–4** · density **2–3**

---

## Cena física

Dono de empresa de serviço, à noite, notebook na mesa. Luz da tela, fundo navy profundo. Humor: foco, cansaço de improviso, decisão de organizar. Não é showroom de tech; é operação séria depois do expediente.

→ Isso **força** dark navy (logo), ouro pontual (decisão/CTA), tipografia geométrica + corpo humano, pouco glow.

---

## Estratégia de cor

**Contida:** neutros tintados no hue da marca + **1 accent ≤10%** da superfície.

| Papel | Hex | OKLCH (approx) | Uso |
|-------|-----|----------------|-----|
| Canvas | `#020226` | `oklch(13% 0.05 275)` | Fundo página |
| Surface | `#0a0a3a` | `oklch(18% 0.06 275)` | Chips método, painéis raros |
| Foreground | `#f7f7f7` | `oklch(97% 0.002 100)` | Títulos e corpo primário |
| Muted | `#9a9ab8` | `oklch(68% 0.04 275)` | Lede, meta, footer |
| Line | `rgba(247,247,247,0.12)` | hairline | Divisores |
| Accent | `#fcc92a` | `oklch(85% 0.16 95)` | CTA, “organizado”, letras do método |

**Proibido:** paleta ANC (glacial/lilás), purple gradients, ouro em faixa larga, texto cinza “lavado” sem chroma do navy.

**Dark justificado:** cena noturna + canvas do logo. Não dark por default SaaS.

---

## Tipografia (máx. 3 famílias)

| Papel | Família | Uso |
|-------|---------|-----|
| Display | **Syne** 700 | H1, H2, labels fortes do método |
| Body | **DM Sans** 400/500/600 | Lede, listas, botões |
| Mono | **IBM Plex Mono** 500 | Kicker, metadados (1 eyebrow max) |

### Escala (direção, não implementação final)

- H1: `clamp(1.65rem, 3.4vw, 2.35rem)` · line-height ~1.18 · tracking ~-0.03em  
  **Duas linhas intencionais:**  
  `Crescimento organizado` / `para empresas de serviços`  
  Ouro em *organizado* só se a frase continuar legível como bloco único.
- H2: ~1.45–1.9rem · max-width ~14ch  
- Body: 17px · line-height 1.55 · max ~40–42ch em prosa  
- Nunca all-caps no corpo; caps só no kicker (≤4 palavras)

---

## Estilo visual (fundamentado)

| Escolha | Por quê |
|---------|---------|
| Dark navy sólido | Logo + cena |
| Accent ouro ≤10% | “O” do wordmark; decisão, não decoração |
| Raios 12–16px | Contido, não over-rounded AI |
| Bordas hairline | Estrutura sem ghost-card |
| Sem glassmorphism default | Anti-slop |
| Sem card grid 3 colunas idêntico | Anti-slop |
| Sem side-stripe dourado | Anti-slop |
| Vídeo no hero | Profundidade real (não orb fake) |
| Copy hero à esquerda | Variance 4, leitura B2B |

**Nível de glow/profundidade:** baixo.  
Profundidade vem do **vídeo + scrim navy**, não de blobs azul/roxo.  
Ouro: botões e ênfase tipográfica, sem glow de botão neon.

---

## Referências reais (ritmo/layout, não copiar paleta)

1. **[releaf.bio](https://releaf.bio/)** — mídia grande + respiro editorial; hero com presença. *Não* copiar light/plant.
2. **João Albano** (`references/joaoalbano`) — densidade tipográfica e hierarquia quieta.
3. **Linear / Vercel-style product dark** (referência de *disciplina*, não de brand) — espaço, tipo, CTA único. Filtrar qualquer accent roxo.
4. **Wordmark Morgen** (`logo-morgen.svg`) — fonte de verdade de cor e proporção.
5. **Constituição Morgen** — tom: simplicidade, tecnologia como meio, sem promessa impossível.

---

## Contato (sistema de conversão visual)

| Canal | Valor | Papel UI |
|-------|--------|----------|
| WhatsApp | +55 21 97062-0150 · `wa.me/5521970620150` | **CTA primário** (ouro) |
| E-mail | morgenagency@gmail.com | CTA secundário / footer |
| Instagram | instagram.com/morgenagencia/ | Footer only |

Mensagem pré-fill WA: `Quero mapear meu crescimento`.

---

## O que a direção *não* é

- Landing ANC recolorida  
- Template SaaS com métricas inventadas  
- Portfólio com cursor magnético / glass / stripe diagonal  
- Página densa tipo “agência 12 seções” (density 2–3)

---

## Revalidação Etapa 2

- [x] Parece premium (contido) e não template genérico? → sim, se ouro ≤10% e type disciplinado  
- [x] Tem identidade própria Morgen? → navy + ouro do logo, método M.O.R.G.E.N.  
- [x] Dark vs light escolhido com propósito? → cena noturna + logo  
- [x] Zero paleta ANC?  
- [x] Tipografia ≤3 famílias?  
- [x] CTA único claro (WhatsApp)?  

---

## Próximo (só após ok humano)

**Etapa 3 — Wireframe** (estrutura de seções density 2–3), depois UI no `index.html`.
