<p align="center">
  <img src="../img/js.svg" width="300">
</p>


## JavaScript

- `addEventListener()` registra uma única espera de evento em um único alvo. O alvo do evento pode ser um único elemento em um documento, o documento em si, uma janela.

- `classList.toggle()` toggle significa alternancia, caso estiver dentro dos parenteses esteja ativo, ele remove, se nao estiver ativo, ele ativa.

- `forEach` percorre cada item de uma lista, array.

Exemplo:

```js
$stars.forEach()
```

BOA PRÁTICA - Toda variável que fazemos referencia ao HTML, colocamos um prefixo, esse prefixo é um `$`

TEMPLATE STRING - Facilita o modo de colocar texto com uma variável. É usado a crase no lugar das aspas e tudo que estiver dentro do `${}` é uma variável.

Exemplo:

```js
`Carrinho(${++valorInicial})`
```
Exemplo:

```js
const { src, alt, nameClass } = card;
```

#### Arrow functions

Exemplo:

```js
() => {}
```

Quando tem apenas um atributo nos parenteses, nao é necessário o uso do mesmo.

Exemplo:

```js
event => {}
```

Valores considerados falsy =  `undefined, null, NaN, 0, -0, string vazia` e todos os outros !== desses é truthy.

Condição ternário = `condição ? true : false`; Ideal para instruções pequenas para melhor leitura.

Método .push() = serve para adicionar itens ao seu Array.

Metodo HOISTING: esse metodo é implicito no javascript e faz a elevação na declaração da função literal. Esse metodo *NAO* funciona se tiver atribuido uma variavel. 
Para evitar esse tipo de problema, é bom colocar as declarações de variavel sempre no começo da função.


```js
function myFunction() {
	function sum(){
		return number1 + number2;}
	var number1 = 1;
	var number2 = 3;
	return sum();
}
console.log( myFunction() );
```

retorno do console = 4.


## JSON - JavaScript Object Notation

Json = `{ propriedade:valor }`
Quando é criada uma função dentro do objeto, é chamado de método.

`Object Destructuring` pega os valores do objeto.