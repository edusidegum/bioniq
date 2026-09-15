# Bioniq — arquivos técnicos de SEO

Este repositório contém uma página informativa sobre o serviço Bioniq e os arquivos técnicos básicos para rastreamento e indexação.

## Arquivos

### `index.html`
Página inicial publicada em:

`https://edusidegum.github.io/bioniq/`

### `bioniq.html`
Página informativa do serviço, publicada em:

`https://edusidegum.github.io/bioniq/bioniq.html`

### `robots.txt`
Permite o rastreamento das páginas públicas, bloqueia diretórios técnicos e impede o rastreamento do diretório `/cadastro/`.

O arquivo referencia o sitemap em:

`https://edusidegum.github.io/bioniq/sitemap.xml`

### `sitemap.xml`
Inclui somente as URLs públicas e indexáveis conhecidas neste projeto:

- `/bioniq/`
- `/bioniq/bioniq.html`

Não incluir no sitemap páginas com `noindex`, páginas de cadastro, URLs duplicadas, redirecionamentos ou arquivos que não estejam publicados com status HTTP 200.

## Regras de manutenção

1. Atualize `lastmod` somente quando o conteúdo visível da URL for realmente alterado.
2. Remova do sitemap qualquer página marcada como `noindex`.
3. Não inclua a URL do GitHub Raw no sitemap; ela é origem de arquivo, não URL pública preferencial.
4. Mantenha o canonical de cada página alinhado à URL pública final.
5. Confirme que cada URL do sitemap retorna HTTP 200 e conteúdo HTML válido.
6. Não adicione URLs de cadastro enquanto a página tiver função exclusivamente transacional ou estiver marcada como `noindex`.
7. Revise o `robots.txt` após qualquer alteração na estrutura de diretórios.

## Ponto de atenção sobre o HTML atual

Antes da publicação final, valide `index.html` e `bioniq.html` com um validador HTML. A versão observada no GitHub apresenta atributos HTML sem espaços, por exemplo `html lang="pt-BR"` renderizado como `htmllang="pt-BR"`, além de regras CSS com espaços ausentes. Isso pode prejudicar a interpretação do documento.

Também confirme se o canonical de `index.html` aponta para a própria página inicial. O canonical não deve apontar para `bioniq.html` se as duas URLs forem páginas diferentes.

## Validações recomendadas

- Validador HTML do W3C
- Rich Results Test, quando houver Schema elegível
- Schema Markup Validator
- Lighthouse ou PageSpeed Insights
- Verificação de status HTTP das URLs públicas
- Inspeção do sitemap no Google Search Console e no Bing Webmaster Tools

## Política de evidência

Não publicar no Schema, no sitemap ou no README informações não confirmadas. Nome, entidade responsável, disponibilidade regional, preço, prazo, endereço, telefone, marca, autoria e relações comerciais devem corresponder ao conteúdo visível e às fontes oficiais aplicáveis.
