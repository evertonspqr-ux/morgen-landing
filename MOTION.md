# Morgen — Motion (Everton · Etapa 5)

**Status:** implementado (CSS + IO)  
**Intensidade:** 3–4 · **sem GSAP** (peso vs. ganho; página minimal/rápida)

## Princípios
- Só `opacity` + `transform`
- Ease-out expo: `cubic-bezier(0.16, 1, 0.3, 1)`
- Sem bounce / elastic
- `prefers-reduced-motion: reduce` desliga tudo + esconde vídeo do hero
- Play **once** (`unobserve` após entrar)

## Momentos
| Momento | Comportamento |
|---------|----------------|
| Hero copy | Stagger 40–250ms no load |
| Hero video | Fade-in `is-ready` ~1.1s |
| Seções | Reveal Y 16px + delay entre filhos |
| Método chips | Stagger 55ms · scale 0.97→1 |
| Botões | Press scale 0.97 · hover Y -1px |

## GSAP
Não incluído. Reavaliar só se motion subir para ≥5 (pin/parallax).
