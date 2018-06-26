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

## Aula 12 - Como usar e suas vantagens/desvantagens? - Como inline
- Imagens não podem ser cacheadas
- Permite edição no DOM
- Animações e Interações de CSS
- Sem requests HTTP adicionais

Exemplo:
```html
<svg version="1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 48 48" enable-background="new 0 0 48 48">
    <g fill="#37474F">
        <path d="M38.5,44.6l-4-4l2.1-2.1l4,4c0.6,0.6,0.6,1.5,0,2.1l0,0C40.1,45.1,39.1,45.1,38.5,44.6z"/>
        <path d="M9.5,44.6l4-4l-2.1-2.1l-4,4c-0.6,0.6-0.6,1.5,0,2.1l0,0C7.9,45.1,8.9,45.1,9.5,44.6z"/>
    </g>
    <circle fill="#C62828" cx="24" cy="24" r="20"/>
    <circle fill="#eee" cx="24" cy="24" r="16"/>
    <rect class="seconds" x="19" y="22.1" transform="matrix(-.707 -.707 .707 -.707 12.904 62.537)" fill="#E53935" width=".8" height="13"/>
    <rect x="23" y="11" width="2" height="13"/>
    <rect x="26.1" y="22.7" transform="matrix(-.707 .707 -.707 -.707 65.787 27.25)" width="2.3" height="9.2"/>
    <circle cx="24" cy="24" r="2"/>
    <circle fill="#C62828" cx="24" cy="24" r="1"/>
    <rect x="22" y="1" fill="#37474F" width="4" height="3"/>
    <g fill="#37474F">
        <path d="M44.4,16.2c2.5-3.5,2.1-8.4-1-11.5c-3.1-3.1-8-3.5-11.5-1L44.4,16.2z"/>
        <path d="M3.6,16.2c-2.5-3.5-2.1-8.4,1-11.5c3.1-3.1,8-3.5,11.5-1L3.6,16.2z"/>
    </g>
</svg>
```
## Aula 13 - A estrutura do SVG - Plano Cartesiano
Informações sobre o eixo `X` e `Ỳ` do plano cartesiano

## Aula 14 - A estrutura do SVG - Viewport e ViewBox
- São propriedades do SVG
- Viewport é o espaço onde vai ocupar o desenho do SVG
- ViewBox é o espaço dentro do Viewport que deverá ser usado. É como se ela desse um zoom in ou zoom out dentro do Viewport

O viewBox possui quatro valores numéricos que podem ser separadas por espaço ou virgula.
```html
viewBox = <min-x> <min-y> <width> <height>
```
São eles:
- min-X: distância mínima do eixo X
- min-Y: distância mínima do eixo Y
- width: é a largura do ViewBox dentro da Viewport
- height: é a altura do ViewBox dentro da Viewport

## Aula 15 - A estrutura do SVG - preserveAspectRatio
- `preserveAspectRatio="none"`: não mantém a proporção
- `<align> [<meetOrSlice>]`:

  Onde `<align>` pode rrerceber os valores:
  - xMinYMin
  - xMidYMin
  - xMaxYMin
  - xMinYMid
  - xMidYMid
  - xMaxYMid
  - xMinYMax
  - xMidYMax
  - xMaxYMax

  E `<meetOrSlice>` pode receber:
  - meet: cobre o máximo que couber sem distorção
  - slice: ocupa o máximo que puder e recorta o restante


  Exemplo:
  ```html
  <svg
      width="400" height="1000"
      viewBox="0 0 230 218"
      preserveAspectRatio="xMaxYMax slice">
<!-- conteúdo do svg -->
  </svg>
  ```

## Aula 16 - A estrutura do SVG - Formas Básicas

- Rect
```html
<svg>
    <rect x="50" y="20" width="100" height="100"/>
</svg>
```

- Circle
```html
<svg>
    <circle r="25" cx="150" cy="70" />
</svg>
```

- Ellipse
```html
<svg>
    <ellipse rx="100" ry="50" cx="150" cy="75" />
</svg>
```

- Line
```html
<svg>
    <line x1="10" y1="10" x2="100" y2="120" stroke="#000" stroke-width="4"/>
</svg>
```

- Polyline
```html
<svg>
    <polyline points="0,40 40,40 40,80 80,80 80,120 120,120, 120,160" fill="transparent" stroke="#000" stroke-width="4"/>
</svg>
```

- Polygon
```html
<svg>
    <polygon points="50,5 100,5 125,30 125,80 100,105 50,105 25,80 25,30" fill="#000" stroke="red" stroke-width="4"/>
</svg>
```

## Aula 17 - A estrutura do SVG - O elemento Path

  - Path

    Valores da propriedade `d`:
    - __M / Moveto__: ponto inicial da curva
    - __L / Lineto__: onde o ponto final vai chegar
    - __A / Arcs__: cria a curva, onde o primeiro valor é A`raio do eixo de x`, `raio do eixo de y` `parâmetro de rotacionamento (normalmente 0)` `concavo/convexo Ex: 0,1` `eixo x`, `eixo y`
    - __z / Closepath__: elemento de fechamento

```html
<svg>
    <path
        stroke="#000"
        stroke-width="4"
        fill="none"
        d="M40,20 L40,80 A30,30 0 1,0 100,100z"
    />
</svg>
```
