# Aprendendo SVG do início ao avançado - Willian Justen

## Aula 01
- [repositório do curso com ementa](https://github.com/willianjusten/curso-de-svg)
- [Projeto Awesome SVG](https://github.com/willianjusten/awesome-svg)
- [Blog do autor com posts sobre SVG](https://willianjusten.com.br/tags/#svg)

## Aula 02
  - História

## Aula 03
  - SVG - Scalable Vector Graphics
  - Imagem vetorial no formato XML
  - Suporta interatividade e animação

## Aula 04
Exemplos de uso:
- https://bl.ocks.org/
- http://panizzon.ind.br/
- https://codepen.io/willianjusten/full/ZYVPep
- http://tutsplus.github.io/Styling-Iconic/styling/

## Aula 05
- Estudar quando se deve usar SVG
- Uso indicado em imagens com poucos detalhes

## Aula 06 - Como criar?
- Illustrator
- Sketch
- Inkscape
- Manualmente com editor de texto

## Aula 07 - Onde baixar?
- Shutterstock
- Vecteezy
- SVG Cuts
- Icomoon
- Iconmonstr
- Material Design Icons
- Iconic
- Flaticon
- Lista na Awesome SVG com mais links

Patterns:
- Plain Pattern
- Trianglify
- SVGeneration
- Pattern bold
- Gerstnerizer

## Aula 08 - Como usar e suas vantagens/desvantagens? - Como Imagem
- Podem ser cacheadas
- Sem interação de CSS
- Sem edição no DOM
- Animações só funcionam se estiverem dentro do SVG

Exemplo:
```html
<img src="img/alarm_clock.svg" alt="Relógio">
```

## Aula 09 - Como usar e suas vantagens/desvantagens? - Como background-image
- Podem ser cacheadas
- Sem interação de CSS
- Sem edição no DOM
- Animações só funcionam se estiverem dentro do SVG

Exemplo:
```html
<style>
.icon {
  display: inline-block;
  width: 500px;
  height: 500px;
}

.icon-music {
  background-image: url(img/audio_file.svg);
}

.icon-clock {
  background-image: url(img/alarm_clock.svg);
}
</style>
<i class="icon icon-music"></i>
```

## Aula 10 - Como usar e suas vantagens/desvantagens? - Como iframe/object/embed
- Bastante lento
- Comportamentos diferentes dependendo do Browser
- Sem permissão de muitas edições, por exemplo manipulação de cores devido a comportamentos diferentes em cada Browser

Exemplo:
```html
<iframe src="img/alarm_clock.svg" frameborder="0"></iframe>

<object data="img/alarm_clock.svg" type=""></object>

<embed src="img/alarm_clock.svg" type="">
```

## Aula 11 - Como usar e suas vantagens/desvantagens? - Como Data URIs
- Não são cacheadas
- Sem interação de CSS
- Sem edição no DOM
- O tamanho pode ser maior que o normal

Exemplo:
```html
<style>
    .icon-clock {
        height: 30px;
        width: 30px;
        background-image: url(data:image/svg+xml;base64,PHN2ZyB2ZXJzaW9uPSIxIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA0OCA0OCIgZW5hYmxlLWJhY2tncm91bmQ9Im5ldyAwIDAgNDggNDgiPgogICAgPGcgZmlsbD0iIzM3NDc0RiI+CiAgICAgICAgPHBhdGggZD0iTTM4LjUsNDQuNmwtNC00bDIuMS0yLjFsNCw0YzAuNiwwLjYsMC42LDEuNSwwLDIuMWwwLDBDNDAuMSw0NS4xLDM5LjEsNDUuMSwzOC41LDQ0LjZ6Ii8+CiAgICAgICAgPHBhdGggZD0iTTkuNSw0NC42bDQtNGwtMi4xLTIuMWwtNCw0Yy0wLjYsMC42LTAuNiwxLjUsMCwyLjFsMCwwQzcuOSw0NS4xLDguOSw0NS4xLDkuNSw0NC42eiIvPgogICAgPC9nPgogICAgPGNpcmNsZSBmaWxsPSIjQzYyODI4IiBjeD0iMjQiIGN5PSIyNCIgcj0iMjAiLz4KICAgIDxjaXJjbGUgZmlsbD0iI2VlZSIgY3g9IjI0IiBjeT0iMjQiIHI9IjE2Ii8+CiAgICA8cmVjdCB4PSIxOSIgeT0iMjIuMSIgdHJhbnNmb3JtPSJtYXRyaXgoLS43MDcgLS43MDcgLjcwNyAtLjcwNyAxMi45MDQgNjIuNTM3KSIgZmlsbD0iI0U1MzkzNSIgd2lkdGg9Ii44IiBoZWlnaHQ9IjEzIi8+CiAgICA8cmVjdCB4PSIyMyIgeT0iMTEiIHdpZHRoPSIyIiBoZWlnaHQ9IjEzIi8+CiAgICA8cmVjdCB4PSIyNi4xIiB5PSIyMi43IiB0cmFuc2Zvcm09Im1hdHJpeCgtLjcwNyAuNzA3IC0uNzA3IC0uNzA3IDY1Ljc4NyAyNy4yNSkiIHdpZHRoPSIyLjMiIGhlaWdodD0iOS4yIi8+CiAgICA8Y2lyY2xlIGN4PSIyNCIgY3k9IjI0IiByPSIyIi8+CiAgICA8Y2lyY2xlIGZpbGw9IiNDNjI4MjgiIGN4PSIyNCIgY3k9IjI0IiByPSIxIi8+CiAgICA8cmVjdCB4PSIyMiIgeT0iMSIgZmlsbD0iIzM3NDc0RiIgd2lkdGg9IjQiIGhlaWdodD0iMyIvPgogICAgPGcgZmlsbD0iIzM3NDc0RiI+CiAgICAgICAgPHBhdGggZD0iTTQ0LjQsMTYuMmMyLjUtMy41LDIuMS04LjQtMS0xMS41Yy0zLjEtMy4xLTgtMy41LTExLjUtMUw0NC40LDE2LjJ6Ii8+CiAgICAgICAgPHBhdGggZD0iTTMuNiwxNi4yYy0yLjUtMy41LTIuMS04LjQsMS0xMS41YzMuMS0zLjEsOC0zLjUsMTEuNS0xTDMuNiwxNi4yeiIvPgogICAgPC9nPgo8L3N2Zz4K);
    }
</style>

<div class="icon-clock"></div>

<img src="data:image/svg+xml;base64,PHN2ZyB2ZXJzaW9uPSIxIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA0OCA0OCIgZW5hYmxlLWJhY2tncm91bmQ9Im5ldyAwIDAgNDggNDgiPgogICAgPGcgZmlsbD0iIzM3NDc0RiI+CiAgICAgICAgPHBhdGggZD0iTTM4LjUsNDQuNmwtNC00bDIuMS0yLjFsNCw0YzAuNiwwLjYsMC42LDEuNSwwLDIuMWwwLDBDNDAuMSw0NS4xLDM5LjEsNDUuMSwzOC41LDQ0LjZ6Ii8+CiAgICAgICAgPHBhdGggZD0iTTkuNSw0NC42bDQtNGwtMi4xLTIuMWwtNCw0Yy0wLjYsMC42LTAuNiwxLjUsMCwyLjFsMCwwQzcuOSw0NS4xLDguOSw0NS4xLDkuNSw0NC42eiIvPgogICAgPC9nPgogICAgPGNpcmNsZSBmaWxsPSIjQzYyODI4IiBjeD0iMjQiIGN5PSIyNCIgcj0iMjAiLz4KICAgIDxjaXJjbGUgZmlsbD0iI2VlZSIgY3g9IjI0IiBjeT0iMjQiIHI9IjE2Ii8+CiAgICA8cmVjdCB4PSIxOSIgeT0iMjIuMSIgdHJhbnNmb3JtPSJtYXRyaXgoLS43MDcgLS43MDcgLjcwNyAtLjcwNyAxMi45MDQgNjIuNTM3KSIgZmlsbD0iI0U1MzkzNSIgd2lkdGg9Ii44IiBoZWlnaHQ9IjEzIi8+CiAgICA8cmVjdCB4PSIyMyIgeT0iMTEiIHdpZHRoPSIyIiBoZWlnaHQ9IjEzIi8+CiAgICA8cmVjdCB4PSIyNi4xIiB5PSIyMi43IiB0cmFuc2Zvcm09Im1hdHJpeCgtLjcwNyAuNzA3IC0uNzA3IC0uNzA3IDY1Ljc4NyAyNy4yNSkiIHdpZHRoPSIyLjMiIGhlaWdodD0iOS4yIi8+CiAgICA8Y2lyY2xlIGN4PSIyNCIgY3k9IjI0IiByPSIyIi8+CiAgICA8Y2lyY2xlIGZpbGw9IiNDNjI4MjgiIGN4PSIyNCIgY3k9IjI0IiByPSIxIi8+CiAgICA8cmVjdCB4PSIyMiIgeT0iMSIgZmlsbD0iIzM3NDc0RiIgd2lkdGg9IjQiIGhlaWdodD0iMyIvPgogICAgPGcgZmlsbD0iIzM3NDc0RiI+CiAgICAgICAgPHBhdGggZD0iTTQ0LjQsMTYuMmMyLjUtMy41LDIuMS04LjQtMS0xMS41Yy0zLjEtMy4xLTgtMy41LTExLjUtMUw0NC40LDE2LjJ6Ii8+CiAgICAgICAgPHBhdGggZD0iTTMuNiwxNi4yYy0yLjUtMy41LTIuMS04LjQsMS0xMS41YzMuMS0zLjEsOC0zLjUsMTEuNS0xTDMuNiwxNi4yeiIvPgogICAgPC9nPgo8L3N2Zz4K" alt="">
```
