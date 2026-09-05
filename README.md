# Vista Malvadex

Versão Vite + React + TypeScript preparada para reproduzir com máxima fidelidade a landing page original criada no GPT Sites, mantendo o CSS editorial, Tailwind/Shadcn base styles, animações, imagens, conteúdo e responsividade do projeto original.

## Rodar localmente

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

A saída é gerada em `dist/`.

## Vercel

- Framework Preset: Vite
- Build Command: `npm run build`
- Output Directory: `dist`
- Install Command: `npm install`

Em um projeto Vite padrão, a Vercel normalmente detecta esses valores automaticamente.

## Compatibilidade de build

O alias `@/` está configurado no TypeScript e no Vite, permitindo imports como `@/lib/utils` no deploy da Vercel. O projeto fixa Node.js 22.x para evitar upgrades automáticos de major.
