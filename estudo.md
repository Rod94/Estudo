# Dicas do Terminal

Lista de comandos que estou aprendendo:

- `cd` (navega entre pastas)
  Exemplo para entrar dentro da pasta:

```
cd nomeDaPasta
```

Exemplo para sair de uma pasta:

```
cd ..
```

- `mkdir` (cria uma nova pasta)
  Exemplo para criar uma nova pasta:

```
mkdir nomeDaPasta
```

- `setas cima ou baixo` vai pegando o histórico ja digitado no terminal.

# Git

- `git init` é usado para inicializar o repositório Git.

- `git status` vê o estado do repositório.

- `git add` vai guardar os itens selecionados que tem na pasta.

- `git add .` vai guardar todos os itens que tem na pasta.

- `git commit -m` é o parametro para passar uma mensagem.

- `git commit -a` parametro para seguir todos os arquivos modificados.

- `git log` lista os arquivos que foram guardados com o `commit`

- `git remote add origin + 'ssh' ou 'https'` serve pra adicionar o link junto ao repositório

- `git push -u origin master` serve para empurrar do repositório local(`master`) para o repositório remoto(`origin`).

- `git commit --amend` vai abrir seu editor com o conteúdo da mensagem do último commit e você pode editar da forma que quiser.

- `git rm -rf "nome do arquivo" --cached` remove do repositorio git mas não remove o arquivo.

# HTML

- `<dl>` descricição de uma lista.
- `<dt>` titulo da descrição.
- `<dd>` definição de uma descrição, tem como padrão `display: block`

# CSS

- `float` o elemento fica flutuando e caso tenha algum elemento abaixo, esse ultimo ocupa o espaço junto com o que foi utilizado o float, sendo que o que foi usado a propriedade float, vai para a frente. Float nunca esconde um conteúdo, o conteúdo define a largura(width) e altura(height) do elemento caso não seja definido. A propriedade float tem o comportamento de tirar do elemento pai, cria um novo contexto.

- `overflow: hidden` essa propriedade esconde o elemento, fazendo com que recalcule o contexto utilizado na propriedade `float`.

- `margin` espaçamento fora dos elementos, respiro externo.
  Formas resumidas:

```
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

## Especificidade de seletores (CSS)

O de baixo sobreescreve o seletor de cima. Valores dos seletores para um melhor entendimento:

seletor id => 100

seletor class / pseudo seletores => 10

seletor tag => 1

# JavaScript

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

- `JSON` JavaScript Object Notation

- `Object Destructuring` pega os valores do objeto.

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
if ternario
condition ? expr1 : expr2 

Se condition é true, o operador retornará o valor de expr1; se não, ele retorna o valor de exp2.