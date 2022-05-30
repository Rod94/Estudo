<p align="center">
  <img src="../img/js.svg" width="300">
</p>


## JavaScript


- `addEventListener()` registra uma única espera de evento em um único alvo. O alvo do evento pode ser um único elemento em um documento, o documento em si, uma janela.

- `classList.toggle()` toggle significa alternancia, caso estiver dentro dos parenteses esteja ativo, ele remove, se nao estiver ativo, ele ativa.

- `forEach` percorre cada item de um array.


BOA PRÁTICA - Toda variável que fazemos referencia ao HTML, colocamos um prefixo, esse prefixo é um `$`

TEMPLATE STRING - Facilita o modo de colocar texto com uma variável. É usado a crase no lugar das aspas e tudo que estiver dentro do `${}` é uma variável.

Exemplo:

```js
let valorInicial = 10
`Carrinho(${valorInicial})`
```

### Arrow functions

Exemplo:

```js
const algumNome = () => {
	return algo;
}
```

Quando tem apenas um parâmetro nos parenteses, nao é necessário o uso do mesmo.

Exemplo:

```js
const algumNome = event => {
	return event;
}
```

Você pode conseguir retornar algo sem a palavra `return` de fato, para isso voce precisa tirar os bigodes e colocar parênteses.

Exemplo:

```js
const algumNome = () => (

)
```

Valores considerados falsy =  `undefined, null, NaN, 0, -0, string vazia` e todos os outros diferentes desses é truthy.

`If ternário`= `condição ? true : false` Ideal para instruções pequenas para melhor leitura.

Método `.push()` = serve para adicionar itens ao seu Array.


```js
const createMemoryCard = ({ alt, nameClass, src }) => 
 `  <article class="memory-card ${nameClass}">
      <img class="icon" src="${src}" alt="${alt}" onClick="handleClick()">
    </article>`;
```
No exemplo acima estou colocando os parametros da função como objeto para que eu possa utiliza-lá passando os valores que eu quiser no momento que eu for chamar a função `createMemoryCard`.

```js
const $memoryCardPHP = createMemoryCard({ src: "img/icon-php.png", alt: "icone php", nameClass: "-front"});
```
E é o que estou fazendo, tenho que observar que para transformar em objeto, preciso usar os bigodes. Isso é chamado de `Object Destructuring` ou `Desestruturação de Objetos`. Tem varias formas que eu posso utiliza-lo.

JSON - JavaScript Object Notation = `{ propriedade: valor }`
Quando é criada uma função dentro do objeto, é chamado de método.