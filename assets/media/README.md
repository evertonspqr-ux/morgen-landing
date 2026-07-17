# Mídia ativa (landing minimal)

| Arquivo | Uso |
|---------|-----|
| `hero-bg.mp4` | Vídeo do hero (~500KB, loop mudo) |
| `hero-poster.jpg` | Poster/LCP (~60KB) |
| `bg-test.mp4` | Original completo (não linkado no HTML) |

Trocar o hero: substitua `hero-bg.mp4` e regenere o poster:
`ffmpeg -y -i hero-bg.mp4 -frames:v 1 -update 1 hero-poster.jpg`
