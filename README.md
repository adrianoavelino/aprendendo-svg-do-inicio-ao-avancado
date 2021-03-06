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


## Aula 18 - A estrutura do SVG - Elementos Containers
  - `<defs>` é um container que possui itens com o intuito de reuso
  - `<g>` é um container responsável por agrupar elementos similares
  - `<symbol>` define um objecto que será instaciado pelo `<use>` e possui viewBox própria

    Exemplos:
    - Defs
      ```xml
      <svg>
          <defs>
              <circle id="meu-circulo" r="25" cx="150" cy="50"/>
          </defs>

          <use xlink:href="#meu-circulo" />
          <use xlink:href="#meu-circulo" x="80" fill="red"/>
      </svg>
    ```

    - g
      ```xml
      <svg>
          <g fill="red">
              <circle id="meu-circulo" r="25" cx="150" cy="50"/>
              <circle id="meu-circulo" r="25" cx="240" cy="50"/>
          </g>
      </svg>
      ```
    - Symbol
      ```xml
      <svg>
          <symbol id="meu-simbolo" viewBox="0 0 150 75">
              <circle r="25" cx="150" cy="50"/>
          </symbol>

          <use xlink:href="#meu-simbolo" />
          <use xlink:href="#meu-simbolo" x="80" fill="red"/>
      </svg>
      ```

## Aula 19 - Estilizando o SVG - Métodos para estililzar pt1
  #### Propriedades de estilo:
  - ***Compartilhado com o CSS***: font, font-size, font-style, font-weight, text-decoration, visibility, color, cursor, display entre outras.

  - ***Exclusivo do SVG***: fill, fill-opacity, stroke, stroke-opacity entre outras


  #### Peso das Propriedades

  Assim como no CSS um estilo pode sobrescrever o outro como no uso de `!important` ou adição de classes em uma TAG, o mesmo ocorre no SVG.

  Ordem dos pesos:
  - User agent: estilos do browser
  - Presentation Attributes: são os atributos colocados diretos na TAG como o width ou height
  - External style: são os estilos externos chamados por link
  - Document styles: são estilos usados dentro dos arquivos HTML na TAG `<style>`
  - Inline styles: são os estilos criados dentro da TAG
  - Animation
  - Override styles: como exemplo temos o `!important`
  - Computed styles:

## Aula 20 - Estilizando o SVG - Métodos para estililzar pt2


### Estilo inline
```xml
<svg style="width: 300px; height:300px;" viewBox="0 0 300 300">
    <polygon
    style="fill: blue; stroke: #ED1C24; stroke-width: 5;"
    points = "279.1,160.8 195.2,193.3 174.4,280.8   117.6,211.1 27.9,218.3 76.7,142.7 42.1,59.6 129.1,82.7 197.4,24.1 202.3,114 "/>
</svg>
```

### Estilo dentro do SVG
```xml
<svg width="300" height="300" viewBox="0 0 300 300">
    <style>
        polygon {
            fill: yellow;
            stroke: #ED1C24;
            stroke-width: 5;
        }
    </style>
    <polygon points = "279.1,160.8 195.2,193.3 174.4,280.8   117.6,211.1 27.9,218.3 76.7,142.7 42.1,59.6 129.1,82.7 197.4,24.1 202.3,114 "/>
</svg>
```
### Estilo fora do SVG
```xml
<style>
    .star {
        fill: green;
        stroke: #ED1C24;
        stroke-width: 5;
    }
</style>

<svg width="300" height="300" viewBox="0 0 300 300">
    <polygon class="star" points = "279.1,160.8 195.2,193.3 174.4,280.8   117.6,211.1 27.9,218.3 76.7,142.7 42.1,59.6 129.1,82.7 197.4,24.1 202.3,114 "/>
</svg>
```

### Estilo externo
```xml
<?xml-stylesheet type="text/css" href="css/main.css"?>
<svg width="300" height="300" viewBox="0 0 300 300">
    <polygon id="star-external" points = "279.1,160.8 195.2,193.3 174.4,280.8   117.6,211.1 27.9,218.3 76.7,142.7 42.1,59.6 129.1,82.7 197.4,24.1 202.3,114 "/>
</svg>
```

## Aula 21 - Estilizando o SVG - Peso das propriedades
Exemplo:
```html

<!DOCTYPE html>
<html>
<head>
    <title>Peso das propriedades</title>
    <link rel="stylesheet" href="css/main.css">
</head>
<body>

<h1>Peso das propriedades</h1>

<style>
    .star {
        fill: green !important;
    }
</style>

<svg width="300" height="300" viewBox="0 0 300 300">
    <polygon style="fill:orange" fill="yellow" class="star" points = "279.1,160.8 195.2,193.3 174.4,280.8   117.6,211.1 27.9,218.3 76.7,142.7 42.1,59.6 129.1,82.7 197.4,24.1 202.3,114 "/>
</svg>

</body>
</html>
```
[Exemplo online](https://willianjusten.com.br/curso-de-svg/estilizando-svg-css/peso-propriedades.html)

## Aula 22 - Estilizando o SVG - Fill e stroke

- __fill__: é o responsável pelo preenchimento do desenhos no SVG
- __fill-opacity__: ele dá opacidade aquele elemento
- __stroke__: é o responsável por fazer o contorno do desenho
- __stroke-width__: é o responsável por aumentar a largura do stroke
- __stroke-dasharray__: transforma o stroke em diversos tracinhos, onde o primeiro valor define o tamanho do tracinho e o segundo o espaço entre os tracinhos (Ex: `stroke-dasharray: 10 5`). Por padrão se a propriedade receber somente um valor ela assume o mesmo valor para  tracinho e o espaço (Ex: `stroke-dasharray: 10`).
- __stroke-dashoffset__: é o responsável sumir com os arrays do `stroke-dasharray`


Através das propriedades  `stroke-dasharray` e `stroke-dashoffset` é possivel criar aquele efeito de estar desenhando alguma coisa na tela. Utillize o [exemplo online](https://willianjusten.com.br/curso-de-svg/estilizando-svg-css/fill-stroke.html) com o developertool alterando os valores para simular o efeito.

## Aula 23 - Estilizando o SVG - Colorindo ícones com mais de uma cor
- através do valor `currentColor` do CSS utilizado na propriedade `fill` é possivel pegar a cor do pai e passar para o `fill`. Quando o `fill` não está definido a cor padrão é preto.
```xml
<path fill="currentColor" d="M24,3C14.6,3,7,10.6,7,20c0,1.2,0,3.4,0,3.4L9,25v-3l21-9.8l9,9.8v3l2-1.6c0,0,0-2.1,0-3.4 C41,12,35.3,3,24,3z"/>
```
- para alterar a cor do fill com o valor `currentColor` deve-se adicionar uma classe ao SVG e dentro da classe CSS deve-se utilizar a propriedade `color`

- para alterar um outro elemento SVG, como um grupo (g), deve-se remover a propriedade `fill` do elemento do SVG e adicionar a propriedade fill numa classe CSS. Dessa forma mantém-se a cor do `currentColor`, somente sobrescreve-se os elementos sem a propriedade fill e com a classe CSS.

Exemplos:
```html
<svg width="320" height="320" class="hidden">
    <symbol id="icon-assistant" viewBox="0 0 48 48">
        <g fill="#FFA726">
            <circle cx="10" cy="26" r="4"/>
            <circle cx="38" cy="26" r="4"/>
        </g>
        <path fill="#FFB74D" d="M39,19c0-12.7-30-8.3-30,0c0,1.8,0,8.2,0,10c0,8.3,6.7,15,15,15s15-6.7,15-15C39,27.2,39,20.8,39,19z"/>
        <path fill="currentColor" d="M24,3C14.6,3,7,10.6,7,20c0,1.2,0,3.4,0,3.4L9,25v-3l21-9.8l9,9.8v3l2-1.6c0,0,0-2.1,0-3.4 C41,12,35.3,3,24,3z"/>
        <g>
            <circle cx="31" cy="26" r="2"/>
            <circle cx="17" cy="26" r="2"/>
        </g>
        <path fill="#757575" d="M43,24c-0.6,0-1,0.4-1,1v-7c0-8.8-7.2-16-16-16h-7c-0.6,0-1,0.4-1,1s0.4,1,1,1h7c7.7,0,14,6.3,14,14v10 c0,0.6,0.4,1,1,1s1-0.4,1-1v2c0,3.9-3.1,7-7,7H24c-0.6,0-1,0.4-1,1s0.4,1,1,1h11c5,0,9-4,9-9v-5C44,24.4,43.6,24,43,24z"/>
        <g fill="var(--primary-color)">
            <path d="M43,22h-1c-1.1,0-2,0.9-2,2v4c0,1.1,0.9,2,2,2h1c1.1,0,2-0.9,2-2v-4C45,22.9,44.1,22,43,22z"/>
            <circle cx="24" cy="38" r="2"/>
        </g>
    </symbol>
</svg>

<style>
    .small {
        width: 100px;
        height: 100px;
        color: red;
        fill: blue;
        --primary-color: black;
    }

    .blue-hair {
        color: blue;
        fill: green;
        transition: color .8s;
        --primary-color: red;
    }

    .blue-hair:hover {
        color: red;
    }
</style>

<svg class="blue-hair">
    <use xlink:href="#icon-assistant" />
</svg>

<svg class="small">
    <use xlink:href="#icon-assistant" />
</svg>

<svg class="small blue-hair">
    <use xlink:href="#icon-assistant" />
</svg>
```

## Aula 24 - Construindo um SVG responsivo e adaptativo - Tornando o SVG fluído

- baixe o seu SVG . Por exemplo no site [Brands of the World](http://www.brandsoftheworld.com)
- otimize no seu editor preferido: agrupando e dividindo em layers
- algumas opoções a serem observadas ao salvar como:
    - SVG profile: SVG 1.1
    - fonts: SVG
    - subsetting: normalmente
    - CSS Properties: Presentation Attributes
    - Decimal places: 1 para SVGs simples e 3 ara complexos
- deixar o SVG responsivo retirando as propriedades width e o height
- para funcionar no IE9 deve-se adicionar a propriedade `preserveAspectRatio="xMidYMid meet"`

## Aula 25 - Construindo um SVG responsivo e adaptativo - Tornando o SVG responsivo e adaptativo

- definir breakpoints (Ex: 1024, 768 e 480)
- utilizar mediaquery no CSS
- adicionar aniamações CSS

```css
<style>
    body {
        background: #240701;
    }
    .container {
        max-width: 700px;
        margin: auto;
        height: 0;
        padding-top: 48%;
        position: relative;
    }
    .svg-responsive {
      position: absolute;
      top: 0;
      left: 0;
    }
    #detalhe-externo,
    #circulo-verde,
    #textos {
        transition: opacity .4s ease-in-out;
    }
    #inner-artwork {
        transition: fill .4s ease-in-out;
    }
    @media(max-width: 768px) {
        #detalhe-externo {
            opacity: 0;
        }
    }
    @media (max-width: 480px) {
        #circulo-verde,
        #textos {
            opacity: 0
        }
        #inner-artwork {
            fill: #067655;
        }
    }
</style>
```

## Aula 26 - Sistema de ícones em SVG - Fixando o uso de ícones com symbol
- baixe alguns SVGs em https://icons8.github.io/flat-color-icons/
- cole o código do SVG no arquivo html
- crie uma symbol dentro do SVG para realizar a inserção do ícones por demanda
- exiba o SVG usando `<use xlink:href="#id-do-symbol">`

```html
<body>
<svg version="1" xmlns="http://www.w3.org/2000/svg">
  <symbol id="icon-approval" viewBox="0 0 48 48">
      <polygon fill="#8BC34A" points="24,3 28.7,6.6 34.5,5.8 36.7,11.3 42.2,13.5 41.4,19.3 45,24 41.4,28.7 42.2,34.5 36.7,36.7 34.5,42.2 28.7,41.4 24,45 19.3,41.4 13.5,42.2 11.3,36.7 5.8,34.5 6.6,28.7 3,24 6.6,19.3 5.8,13.5 11.3,11.3 13.5,5.8 19.3,6.6"/>
      <polygon fill="#CCFF90" points="34.6,14.6 21,28.2 15.4,22.6 12.6,25.4 21,33.8 37.4,17.4"/>
    </symbol>
    <symbol id="icon-about" viewBox="0 0 48 48">
        <path fill="#2196F3" d="M37,40H11l-6,6V12c0-3.3,2.7-6,6-6h26c3.3,0,6,2.7,6,6v22C43,37.3,40.3,40,37,40z"/>
        <g fill="#fff">
            <rect x="22" y="20" width="4" height="11"/>
            <circle cx="24" cy="15" r="2"/>
        </g>
    </symbol>
    <symbol id="icon-automatic" viewBox="0 0 48 48">
        <path fill="#3F51B5" d="M39,43H9c-2.2,0-4-1.8-4-4V9c0-2.2,1.8-4,4-4h30c2.2,0,4,1.8,4,4v30C43,41.2,41.2,43,39,43z"/>
        <path fill="#B3E5FC" d="M33.6,25.4c0.1-0.4,0.1-0.9,0.1-1.4s0-0.9-0.1-1.4l2.8-2c0.3-0.2,0.4-0.6,0.2-0.9l-2.7-4.6 c-0.2-0.3-0.5-0.4-0.8-0.3L30,16.3c-0.7-0.6-1.5-1-2.4-1.4l-0.3-3.4c0-0.3-0.3-0.6-0.6-0.6h-5.3c-0.3,0-0.6,0.3-0.6,0.6L20.4,15 c-0.9,0.3-1.6,0.8-2.4,1.4l-3.1-1.4c-0.3-0.1-0.7,0-0.8,0.3l-2.7,4.6c-0.2,0.3-0.1,0.7,0.2,0.9l2.8,2c-0.1,0.4-0.1,0.9-0.1,1.4 s0,0.9,0.1,1.4l-2.8,2c-0.3,0.2-0.4,0.6-0.2,0.9l2.7,4.6c0.2,0.3,0.5,0.4,0.8,0.3l3.1-1.4c0.7,0.6,1.5,1,2.4,1.4l0.3,3.4 c0,0.3,0.3,0.6,0.6,0.6h5.3c0.3,0,0.6-0.3,0.6-0.6l0.3-3.4c0.9-0.3,1.6-0.8,2.4-1.4l3.1,1.4c0.3,0.1,0.7,0,0.8-0.3l2.7-4.6 c0.2-0.3,0.1-0.7-0.2-0.9L33.6,25.4z M24,29c-2.8,0-5-2.2-5-5c0-2.8,2.2-5,5-5c2.8,0,5,2.2,5,5C29,26.8,26.8,29,24,29z"/>
    </symbol>
</svg>

<svg>
  <use xlink:href="#icon-approval" />
</svg>

<svg>
  <use xlink:href="#icon-about" />
</svg>

<svg>
  <use xlink:href="#icon-automatic" />
</svg>
</body>
```
- salve o conteúdo do svg num arquivo chamado **symbols.svg**
- modifique as tags `<use xlink:href="#id-do-symbol">` conforme o exemplo abaixo:

```html
<svg>
  <use xlink:href="symbols.svg#icon-approval" />
</svg>

<svg>
  <use xlink:href="symbols.svg#icon-about" />
</svg>

<svg>
  <use xlink:href="symbols.svg#icon-automatic" />
</svg>
```

## Aula 27 - Sistema de ícones em SVG - Usando o Icomoon
- acesse o site https://icomoon.io/app/
- importe os arquivos SVG
- clique em ***Generate SVG or more***
