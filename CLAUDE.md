# CLAUDE.md — FASHION4FUN

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** FASHION4FUN
**Nicho:** Moda e Beleza
**Keywords:** Sobre Nos Somos duas Duas amantes de moda claro Duas mulheres corajosas
**Paleta de cores:** teal | **Fonte:** inter

Sobre Nós Somos duas. Duas amantes de moda, claro. Duas mulheres corajosas e afrente do seu tempo também, assim como todos buscando um sonho de fazer algo que ame, com propósito. Duas pessoas que amam roupa, se expressar, cores e tudo que o mundo da moda oferece. Mostramos nossa perspectiva sobre diversos assuntos nesse site, pelo nosso blog. Confira alguns.   Nosso Time Sobre Nós Renata Fernandes Fotografia Influenciada por um pai fotografo, venho desde garota nutrindo meu amor por fotografia, que quando mais velha se assumiu um amor maior ainda por moda. Me formei na Puc-Rio no final de 2018. Sou muito grata de desde então por estar trabalhando ao lado de uma pessoa incrível que nem a Sabrina Sobre Nós Sabrina Trindade Designer de Moda Formada pela Unirio em 2016 vim buscando no meu mercado me tornar uma profissional realizada, através do blog fashion 4 fun venho conseguindo criar amigos e clientes apaixonados por moda.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-F |
| Hero | Hero-H |
| Features | Features-F |
| About Section | About-G |
| Posts | Posts-A |
| Footer | Footer-G |
| Página Sobre | Sobre-A |
| Página Contato | Contato-F |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
