# Mídia ativa (landing minimal)

| Arquivo | Uso |
|---------|-----|
| `hero-bg.mp4` | Vídeo do hero (~500KB, loop mudo) |
| `hero-poster.jpg` | Poster/LCP (~60KB) |
| `og.jpg` | Open Graph 1200×630 |

Trocar o hero: substitua `hero-bg.mp4` e regenere poster + OG:
```bash
ffmpeg -y -i hero-bg.mp4 -frames:v 1 -update 1 hero-poster.jpg
# depois regerar og.jpg a partir do poster (ver pipeline / AUDIT)
```
