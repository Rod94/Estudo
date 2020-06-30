# CSS

- `float` o elemento fica flutuando e caso tenha algum elemento abaixo, esse ultimo ocupa o espaço junto com o que foi utilizado o float, sendo que o que foi usado a propriedade float, vai para a frente. Float nunca esconde um conteúdo, o conteúdo define a largura(width) e altura(height) do elemento caso não seja definido. A propriedade float tem o comportamento de tirar do elemento pai, cria um novo contexto.

- `overflow: hidden` essa propriedade esconde o elemento, fazendo com que recalcule o contexto utilizado na propriedade `float`.

- `margin` espaçamento fora dos elementos, respiro externo.
  Formas resumidas:

```css
margin: top right bottom left;
margin: top/bottom right/left;
margin: top right/left bottom;
margin: top/right/bottom/left;
```

- `padding` espaçamento dentro dos elementos, respiro interno.
  Formas resumidas:

```css
padding: top right bottom left;
padding: top/bottom right/left;
padding: top right/left bottom;
padding: top/right/bottom/left;
```

- `display: inline;` deixa elementos na mesma linha, nessa propriedade não conseguimos colocar width e height. Ele ganha o comportamento de uma palavra, um conteúdo.

- `display: block;` não deixa elementos na mesma linha, nessa propriedade conseguimos colocar width e height.

- `display: inline-block;` consegue deixar elementos na mesma linha e conseguimos definir width e height. Ele ganha o comportamento de uma palavra, um conteúdo.

- `position: absolute;` ele cria um novo contexto, ficando na frente de todos na tela, o que define width e height é o conteúdo dentro dele, com `top, left, right, bottom` é possivel mover em relação a pagina.

- `box-sizing` padrão é `content-box`, colocando `border-box` o que voce informou no de width/height, é o que ele utiliza, já no `content-box`, ele absorve se você colocou alguma borda.

- `max-width` serve pra colocar o maximo de largura que o site vai ter para a tela

- `@media` sempre que ver algum `breakpoint`(quando o site quebra linhas e muda o layout do site) é usado essa propriedade.

- Para conseguir utilizar o `margin: auto`, o elemento tem que ser `display: block` tem que ter um `width`(largura) definida.

- Para tirar o sublinhado do `<a></a>` é só colocar `text-decoration: none;`

## Especificidade de seletores (CSS)

O de baixo sobreescreve o seletor de cima. Valores dos seletores para um melhor entendimento:

seletor id => 100

seletor class / pseudo seletores => 10

seletor tag => 1

## ITCSS com React

- Pasta SETTINGS: contém variáveis nos arquivos de cores, de tamanho e espaçamento, podem ter mais coisas, mas geralmente é o que tem nessa pasta.

- Pasta TOOLS: são funções que mexem com o comportamento de outros arquivos. Exemplos: centralizar, botar para o lado direito ou esquerdo.

- Pasta GENERIC: tem o arquivo reset.css

- Pasta ELEMENTS/BASE: mexer o comportamento padrão das tags.