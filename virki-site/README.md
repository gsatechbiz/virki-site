# VIRKI Special Solutions — Site

Site estático multi-idioma para deploy via Cloudflare Pages.

## Estrutura

```
virki-site/
├── index.html          → PT-BR (raiz)
├── en/
│   └── index.html      → EN
├── es/
│   └── index.html      → ES
├── assets/
│   └── logo-virki-claro.png
├── _redirects          → regras Cloudflare Pages
└── README.md
```

## Deploy no Cloudflare Pages

1. Crie um repositório no GitHub e faça push desta pasta.
2. No Cloudflare Pages → Create a project → Connect to Git.
3. Selecione o repositório.
4. Build settings:
   - **Framework preset:** None
   - **Build command:** (deixar vazio)
   - **Build output directory:** `/` (raiz)
5. Deploy.

## Imagens placeholder

As fotos atuais usam `picsum.photos`. Substituir pelos caminhos reais em `assets/` quando disponíveis — basta trocar o `src` nas três versões do `index.html`.

## Idioma ativo no seletor

Cada versão já marca o idioma correto como `.active` na nav e no painel mobile.
