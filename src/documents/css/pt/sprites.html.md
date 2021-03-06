---
order: 1
title: Use CSS Sprites
---

Essa técnica consiste em agrupar diversas imagens em uma só.

<img id="img-sprite" src="http://assets.browserdiet.com/img/sprite-example.jpg" alt="CSS Sprite Example" width="483" height="21">

E depois posicioná-las através de CSS.

```css
.icon-foo {
  background-image: url('mySprite.png');
  background-position: -10px -10px;
}

.icon-bar {
  background-image: url('mySprite.png');
  background-position: -5px -5px;
}
```

Isso faz com que diminua absurdamente o número de requisições HTTP e evite atrasos no download de outros recursos da sua página.

Ao montar seu *sprite*, evite deixar muito espaço em branco entre as imagens, isso não afeta o peso do arquivo, mas sim o uso de memória para processar o mapa de pixels.

Apesar de extremamente difundida, essa técnica é pouco usada já que os desenvolvedores não utilizam ferramentas que automatizam o processo de geração dessa imagem. Por isso, separamos algumas que podem te ajudar nisso.

 *> Ferramentas úteis: [SpritePad](http://wearekiss.com/spritepad), [Compass](http://compass-style.org/help/tutorials/spriting/), [SpriteMe](http://www.spriteme.org/) e [Sprite Cow](http://www.spritecow.com/).*
