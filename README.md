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
