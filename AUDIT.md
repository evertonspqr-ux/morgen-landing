# Morgen — Auditoria final (Everton · Etapas 6–8 + 10)

**Branch:** `feat/media-mockup`  
**Data:** 2026-07-17  
**Stack:** static HTML/CSS/JS (opção 1 do pipeline)

---

## Etapa 6 — 3D / Parallax

| Item | Decisão |
|------|---------|
| TiltCard / fake 3D | **Skip** |
| Parallax scroll | **Skip** |
| Hero orbs ANC | **Skip** (anti-slop + brand) |
| Profundidade | Vídeo + scrim navy + poster |

**Motivo:** density 2–3, “rápido”, variance 4 já coberta por hero assimétrico. Motion ≥7 exigiria GSAP; dial está em 3–4.

---

## Etapa 7 — Vídeo e mídia

| Item | Status |
|------|--------|
| `hero-bg.mp4` | ~500KB, 720p, mudo, loop, corte 1.1s na origem |
| `hero-poster.jpg` | Frame estático ~60KB, preload |
| `poster` + CSS background | LCP sem esperar vídeo |
| `preload="none"` + `data-src` | Carrega sob demanda |
| Skip vídeo | `prefers-reduced-motion`, saveData, 2g, CPU ≤2 |

---

## Etapa 8 — Performance

| Check | Status |
|-------|--------|
| Fonts `display=swap` | sim |
| Preconnect Google Fonts | sim |
| Preload poster | sim |
| Vídeo não bloqueia LCP | sim (poster primeiro) |
| Dual-video / GSAP | não (peso) |
| `bg-test.mp4` original 3.7MB | mantido em assets (não linkado no HTML) |

**Alvos (manual no PageSpeed quando deployar):** mobile ≥85, LCP ≤2.5s, CLS ≤0.1.

---

## Etapa 9 — Transições de página

N/A (single page).

---

## Etapa 10 — Checklist

### Conteúdo e conversão
- [x] Hero com promessa em ~3s
- [x] CTA óbvio (WhatsApp) nav + hero + fim
- [x] Copy sem jargão AI / sem em-dash
- [x] WA: `https://wa.me/5521970620150?text=...`
- [x] E-mail + Instagram no footer

### Visual e identidade
- [x] Reveals nas seções
- [x] Scroll smooth (respeita reduced-motion)
- [x] Parallax: skip consciente
- [x] Hover em botões e links de footer
- [x] Paleta Morgen (não ANC)
- [x] 1 eyebrow (hero only)

### Anti-slop
- [x] Sem gradient text
- [x] Sem side-stripe
- [x] Sem glass default
- [x] Sem hero-metrics inventados
- [x] Sem card grid idêntico
- [x] Sem cursor magnético
- [x] Sem stripe backgrounds

### Técnico
- [x] Static (sem Framer/Next pitfalls)
- [x] SEO description + OG básicos
- [x] Contatos reais documentados

---

## Pipeline status

| # | Etapa | Status |
|---|--------|--------|
| 1 | Estratégia | done |
| 2 | Direção de arte | done (`DESIGN-DIRECTION.md`) |
| 3 | Wireframe | done (`WIREFRAME.md`) |
| 4 | UI/UX | done (`index.html`) |
| 5 | Motion | done (`MOTION.md`) |
| 6 | 3D/parallax | skip documentado |
| 7 | Vídeo | done |
| 8 | Performance | done |
| 9 | Page transitions | N/A |
| 10 | Auditoria | este arquivo |

---

## Pós-pipeline (deploy)

1. [x] Merge `feat/media-mockup` → `main`  
2. [x] OG image `assets/media/og.jpg` + meta tags  
3. [x] Removido `bg-test.mp4` / `case-loop` (peso)  
4. [x] Bloco honestidade (marca nova, sem cases)  
5. [x] Favicon + apple-touch + robots.txt + sitemap + JSON-LD  
6. [ ] Prova social real quando houver o 1º case  
7. [ ] Domínio custom (se houver)  

**Pages:** https://evertonspqr-ux.github.io/morgen-landing/  


