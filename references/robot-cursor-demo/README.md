# Robô que segue o cursor (como joaoalbano.com)

## O que os caras usam

Não é mágica custom em canvas puro. No bundle React deles:

```js
heroVisual: {
  type: "spline",
  scene: "https://prod.spline.design/kZDDjO5HuC9GJUM2/scene.splinecode"
}
```

Stack:
1. **[Spline](https://spline.design)** — modelagem 3D + eventos (mouse look-at, idle, etc.)
2. Runtime no site: `@splinetool/viewer` / `@splinetool/react-spline` + **Three.js** por baixo
3. O “seguir cursor” é **configurado na cena Spline** (events → look at mouse / variables)

Arquivo da cena (1.3 MB): `scene.splinecode` (baixado de prod.spline.design).

## Demo local

```bash
cd /home/atlas/projetos/morgen-landing/references/robot-cursor-demo
python3 -m http.server 8771 --bind 127.0.0.1
# http://127.0.0.1:8771
```

## Como a Morgen deve fazer (certo)

1. Abrir [spline.design](https://spline.design) (conta free)
2. Importar / criar robô (ou remix de um template humanoid)
3. Em **Events**: Mouse move → Look at / Rotate toward pointer
4. Export **Code** → copiar URL `*.splinecode` ou baixar o arquivo
5. Embed:

```html
<script type="module" src="https://unpkg.com/@splinetool/viewer/build/spline-viewer.js"></script>
<spline-viewer url="SUA_CENA.splinecode"></spline-viewer>
```

Ou React:

```bash
npm i @splinetool/react-spline
```

```jsx
import Spline from '@splinetool/react-spline';
<Spline scene="https://prod.spline.design/SEU_ID/scene.splinecode" />
```

## Alternativas (sem Spline)

| Opção | Prós | Contras |
|-------|------|---------|
| Spline (igual a eles) | Rápido, visual, eventos prontos | Depende da plataforma |
| Three.js + GLB próprio | 100% teu, offline | Mais engenharia (lookAt mouse) |
| Lottie 2D | Leve | Não é 3D “surreal” |

## Aviso

A cena `kZDDjO5HuC9GJUM2` é **asset deles** — use só como referência técnica.
Para produção Morgen, crie/compre modelo próprio e hospede o `.splinecode` ou `.glb` no vosso domínio/repo.
