# Malvadex — Landing Page

Landing page institucional da **Malvadex (MVDX)**, loja de streetwear em Vila Velha — ES.

O projeto foi preparado para versionamento em GitHub sem dependências instaladas, caches, arquivos de build ou metadados locais de hosting.

## Stack

- React 19
- TypeScript 5
- Vinext
- Vite 8
- Tailwind CSS 4
- Lucide React

## Requisitos

- Node.js **22.13 ou superior**
- pnpm compatível com lockfile v9 (pnpm 9+)

Com Node.js instalado, você pode habilitar o Corepack antes de usar o pnpm:

```bash
corepack enable
```

## Rodar localmente

```bash
pnpm install
pnpm dev
```

Depois, abra o endereço exibido pelo terminal.

## Scripts

```bash
pnpm dev      # ambiente de desenvolvimento
pnpm build    # build de produção
pnpm start    # executa o build via Wrangler
pnpm lint     # análise estática com Oxlint
pnpm format   # formatação com Oxfmt
```

## Build de produção

```bash
pnpm install --frozen-lockfile
pnpm build
```

A saída estática é gerada em:

```text
dist/client
```

## Publicar o código no GitHub

Crie um repositório vazio no GitHub e, dentro desta pasta, execute:

```bash
git init
git add .
git commit -m "Initial commit: Malvadex landing page"
git branch -M main
git remote add origin https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
git push -u origin main
```

Substitua `SEU-USUARIO` e `SEU-REPOSITORIO` pelos dados do seu repositório.

## Deploy

O projeto gera uma saída estática em `dist/client`, portanto pode ser integrado a provedores de hospedagem que aceitem um comando de build e uma pasta de saída.

Configuração típica:

- **Build command:** `pnpm build`
- **Output directory:** `dist/client`
- **Node:** 22.13+

### GitHub Pages

O código pode ficar normalmente no GitHub. Para hospedar o site em um **Project Page** (`usuario.github.io/repositorio/`), será necessário adaptar o base path porque o projeto atualmente usa caminhos absolutos como `/images/...`.

Se o site usar um domínio próprio ou for servido na raiz do domínio, essa limitação não se aplica.

## Estrutura principal

```text
app/                  páginas, layout e estilos globais
components/           componentes reutilizáveis
hooks/                hooks React
lib/                  utilitários
public/               favicon e imagens do site
scripts/build.cjs     script de build Vinext
IMAGE-SOURCES.json    origem/créditos das imagens utilizadas
```

## Conteúdo e direitos

Este repositório está marcado como `UNLICENSED`. As imagens e elementos visuais pertencem aos respectivos autores/proprietários e não são disponibilizados como conteúdo open source.

Os créditos e referências das imagens utilizadas estão registrados em `IMAGE-SOURCES.json`.

## Observações

- Nenhum arquivo `.env` ou credencial é necessário no estado atual do projeto.
- Metadados específicos do hosting original em OpenAI Sites foram removidos da versão preparada para GitHub.
- Antes de publicar mudanças em produção, confirme endereço, telefone, links sociais e horários comerciais exibidos na página.
