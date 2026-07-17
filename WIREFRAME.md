# Morgen — Wireframe (Everton · Etapa 3)

**Status:** aguardando aprovação  
**Dials:** variance 4 · motion 3–4 · density 2–3  
**Base:** Etapa 1 (estratégia) + Etapa 2 (`DESIGN-DIRECTION.md`)

---

## Ritmo de scroll

```
impacto (hero) → respiro (problema) → clareza (solução)
→ método (sequência) → conversão (CTA) → saída (footer)
```

Nada só para preencher. Sem prova social inventada, pricing, FAQ, marquee de logos, métricas fake.

---

## Mapa de seções

### 0. Nav (sticky)
| Zona | Conteúdo |
|------|----------|
| Esq. | Logo wordmark (link `#topo`) |
| Dir. | CTA primário → WhatsApp `Falar com a Morgen` |

Mobile: logo + CTA (sem menu hambúrguer; poucas seções, âncoras opcionais depois se precisar).

---

### 1. Hero (`#topo`) — impacto
| Camada | Conteúdo |
|--------|----------|
| Fundo | Vídeo `hero-bg.mp4` full-bleed do bloco · mudo · loop · scrim navy |
| Copy | Colada à **esquerda** (pad da página) |
| Kicker | `Aquisição + automação` (único eyebrow da página) |
| H1 | 2 linhas: `Crescimento organizado` / `para empresas de serviços` |
| Lede | 1–2 frases: captar + atender + menos manual; tecnologia como meio |
| Ações | Primary: `Quero mapear meu crescimento` → WA · Ghost: `Ver o método` → `#metodo` |

**Não:** slot 3D, métricas, dual-column com card vazio.

---

### 2. Problema (`#problema`) — respiro
| Elemento | Conteúdo |
|----------|----------|
| H2 | `Onde o crescimento trava` |
| Lista vertical | 4 itens (título + 1 linha muted), hairline entre eles |

Itens (da Constituição):
1. Poucos clientes  
2. Atendimento lento  
3. Processo manual  
4. Oportunidades perdidas  

Layout: single column, max ~32–34rem. Sem ícones, sem grid 2×2 de cards.

---

### 3. Solução (`#solucao`) — clareza
| Elemento | Conteúdo |
|----------|----------|
| H2 | `O que a Morgen faz` |
| Intro | 2–3 linhas: sistemas + operação; não anúncio solto / “mais ferramenta” |
| Lista de 3 | stack vertical com **respiro** (não side-stripe, não card grid idêntico) |

1. **Captar com estrutura**  
2. **Automatizar o que já funciona**  
3. **Reduzir trabalho manual**  

---

### 4. Método (`#metodo`) — sequência (numeração ok: ordem importa)
| Elemento | Conteúdo |
|----------|----------|
| H2 | `Método M.O.R.G.E.N.` |
| Chips | M · O · R · G · E · N (Mapear… Nutrir) em linha que quebra |
| Nota | 1 frase: sair do improviso, crescimento que a operação aguenta |

Stagger de entrada na Etapa 5. Sem diagrama placeholder obrigatório (density 2).

---

### 5. CTA final (`#contato`) — conversão
| Elemento | Conteúdo |
|----------|----------|
| H2 | `Vamos mapear o que trava o seu crescimento` |
| Apoio | `Conversa direta. Diagnóstico primeiro, sistema depois.` |
| Ações | Primary ouro: **Falar no WhatsApp** · Ghost: **Enviar e-mail** |

Links:
- `https://wa.me/5521970620150?text=Quero%20mapear%20meu%20crescimento`
- `mailto:morgenagency@gmail.com?subject=Quero%20mapear%20meu%20crescimento`

---

### 6. Footer
| Esq. | Dir. |
|------|------|
| Logo | e-mail · WA (+55 21 97062-0150) · Instagram · © ano |

---

## Esqueleto ASCII (desktop)

```
┌─────────────────────────────────────────────┐
│ [LOGO]                    [Falar c/ Morgen] │  nav
├─────────────────────────────────────────────┤
│ ░░░░░░░░░░░░░ VIDEO + SCRIM ░░░░░░░░░░░░░░░ │
│ Texto………………                                │  hero
│ H1 linha 1                                  │
│ H1 linha 2                                  │
│ lede…                                       │
│ [Mapear] [Método]                           │
├─────────────────────────────────────────────┤
│ Onde o crescimento trava                    │
│ ─ item                                      │
│ ─ item                                      │
│ ─ item                                      │
│ ─ item                                      │
├─────────────────────────────────────────────┤
│ O que a Morgen faz                          │
│ intro…                                      │
│ Captar…                                     │
│ Automatizar…                                │
│ Reduzir…                                    │
├─────────────────────────────────────────────┤
│ Método M.O.R.G.E.N.                         │
│ [M][O][R][G][E][N]                          │
│ nota…                                       │
├─────────────────────────────────────────────┤
│ CTA final                                   │
│ [WhatsApp] [E-mail]                         │
├─────────────────────────────────────────────┤
│ logo    mail · wa · ig · ©                  │
└─────────────────────────────────────────────┘
```

---

## Mobile (repensado, não só encolhido)

- Hero min-height menor (~70vh); copy ainda left + pad  
- CTAs full-width empilhados se necessário  
- Chips método wrap natural  
- Footer links em coluna ou wrap  
- Nav: logo menor + CTA compacto  

---

## Fora do escopo deste wireframe

| Item | Motivo |
|------|--------|
| Prova social / logos | Sem assets reais ainda |
| Pricing | Ticket consultivo, não self-serve |
| FAQ | Density 2; só se bloquear conversão depois |
| Bento 3D / slots | Mockup antigo; não no path minimal |
| Dual video A/B | Performance |

---

## Revalidação Etapa 3

- [x] Scroll com ritmo: impacto → respiro → prova de clareza → método → CTA?  
- [x] Nada só para preencher?  
- [x] CTA óbvio (WA) no nav + fim?  
- [x] Narrativa alinhada à Constituição?  
- [x] Density 2–3 respeitada?

---

## Próximo (após ok)

**Etapa 4 — UI/UX:** aplicar este wireframe + direção de arte no `index.html` (hierarquia, hover, mobile).
