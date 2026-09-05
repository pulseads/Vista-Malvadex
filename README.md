# Vista Malvadex

Landing page da Malvadex convertida para uma estrutura padrão **Vite + React + TypeScript**, pronta para GitHub e deploy automático na Vercel.

## Rodar localmente

Requer Node.js 22.13 ou superior.

```bash
npm install
npm run dev
```

## Build de produção

```bash
npm run build
```

A saída é gerada em `dist/`.

## Deploy na Vercel

Ao importar o repositório na Vercel, ela deve detectar Vite automaticamente.

- Framework Preset: `Vite`
- Build Command: `npm run build`
- Output Directory: `dist`
- Install Command: `npm install`

Normalmente não é necessário preencher esses campos manualmente.

## GitHub Desktop

Depois de substituir os arquivos no repositório local:

1. Abra o repositório no GitHub Desktop.
2. Confira as alterações em **Changes**.
3. Crie um commit, por exemplo: `Convert project to standard Vite`.
4. Clique em **Push origin**.
5. A Vercel fará um novo deploy automaticamente se o repositório já estiver conectado.

## Estrutura

```text
src/
  components/
    Motion.tsx
  App.tsx
  main.tsx
  styles.css
public/
  images/
  favicon.svg
index.html
package.json
vite.config.ts
```

## Observações

- O layout, conteúdo, imagens, links, mapa, animações e responsividade do projeto original foram preservados.
- Dependências e metadados específicos do OpenAI Sites/Vinext foram removidos.
- As fontes Bodoni Moda e Inter Tight são carregadas pelo Google Fonts no `index.html`.
