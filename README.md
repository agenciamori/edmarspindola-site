# Dr. Edmar Spindola — Transplante Capilar Altamira

Site institucional do Dr. Edmar Spindola, dermatologista especialista em transplante capilar em Altamira, PA.

**URL de produção:** https://transplantecapilaraltamira.com.br

## Stack

HTML/CSS/JS estático puro, sem framework, sem build step. Hospedado no Netlify.

## Estrutura

Cada pasta é uma URL limpa (ex: `/masculino/index.html` → `transplantecapilaraltamira.com.br/masculino`). A Home fica na raiz.

```
index.html                     → /
edmar-spindola/                → /edmar-spindola
casos/                         → /casos
contato/                       → /contato
avaliacoes/                    → /avaliacoes
perguntas-frequentes/          → /perguntas-frequentes
clinica-altamira/              → /clinica-altamira
privacidade/                   → /privacidade
masculino/                     → /masculino
feminino/                      → /feminino
barba/                         → /barba
sobrancelha/                   → /sobrancelha
metodos/                       → /metodos
metodos/fue-tradicional/       → /metodos/fue-tradicional
metodos/fue-no-shave/          → /metodos/fue-no-shave
metodos/dhi/                   → /metodos/dhi
blog/                          → /blog
blog/o-que-e-tecnica-fue/      → /blog/o-que-e-tecnica-fue

styles.css                     → folha de estilo única, compartilhada por todo o site
img/                           → imagens (ver MANIFESTO-FOTOS.txt)
robots.txt, sitemap.xml, llms.txt → arquivos técnicos de SEO/GEO, precisam ficar na raiz
```

## Convenções importantes

- **Todo link interno usa caminho absoluto** (`/masculino`, `/styles.css`), nunca relativo. Isso é obrigatório por causa da estrutura de pastas — um link relativo quebra dependendo de qual pasta a página está.
- **Toda imagem também usa caminho absoluto** (`/img/nome-do-arquivo.jpg`). Nomes e legendas (alt text) esperados estão listados em `MANIFESTO-FOTOS.txt`.
- Header/rodapé são idênticos em todas as páginas (mesmo bloco de HTML repetido). Qualquer mudança nesses componentes precisa ser replicada nas 18 páginas.

## Como atualizar

Esse repositório está conectado ao Netlify. Qualquer alteração enviada (commit) pra branch principal republica o site automaticamente em produção, sem passo manual.

## Pendências conhecidas

- Espaços de vídeo vertical (Masculino, Feminino, Barba, Sobrancelha, Avaliações, Casos) ainda aguardando link de embed
- Fotos reais ainda pendentes — ver `MANIFESTO-FOTOS.txt` pra lista completa de arquivos esperados em `img/`
- 2 artigos do blog ainda sem página própria (cards existem em `/blog`, sem link ativo ainda)
