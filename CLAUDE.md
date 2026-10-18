# SiteJogos

Página inicial que lista os jogos publicados: https://parappathe.github.io/ (repositório
`parappathe.github.io` no GitHub). Cada jogo é publicado no próprio repositório e fica em
`https://parappathe.github.io/<Projeto>/`; esta página só tem os links.

## Como rodar / testar

`python -m http.server 8767` nesta pasta e abrir `http://localhost:8767` (`.claude/launch.json`).
Os links dos jogos só funcionam no site publicado (são caminhos relativos ao domínio).

## Como publicar

Na pasta `C:\claude code`: `python publicar.py SiteJogos --repo parappathe.github.io`.

## Estrutura

| Arquivo | O que tem |
|---|---|
| `index.html` | A página inteira (estilo embutido; capas dos jogos desenhadas em SVG) |
| `.nojekyll` | Faz o GitHub servir os arquivos como estão |

## Regras e convenções do projeto

- Jogo novo publicado: acrescentar um cartão (`<a class="game">`) no `index.html`, com link
  relativo `NomeDoRepositorio/`, e republicar esta página.
- Letras e botões grandes: a página é usada no navegador do Quest.

## Decisões

- Um repositório por jogo (cada projeto continua independente) + este repositório como
  página inicial, todos no mesmo domínio `parappathe.github.io`.
- Título neutro ("Sala de Jogos"), sem nome completo, porque o site é público.

## Pendências / problemas conhecidos

- Nenhuma.
