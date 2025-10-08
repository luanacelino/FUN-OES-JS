# FuncoesJS

Na ultima aula aprendemos sobre funções, como criar-las utilizando formatos como: declaration, expression e arrow. Primeiro, devemos entender o que é uma função e como ela se comporta. 

As funções te permitem uma melhor organização, escalabilidade e eficiencia do codigo. As funções são um conjunto de codigos reutilizaveis e são executadas quando "chamadas" ou "invocadas". Ex:
```js
function minhaFuncao(p1, p2) {
  return p1 * p2;
}
```
Em seguida, devemos entender como é a sintaxe da função em JS. Uma função é definida com a palavra-chave FUNCTION, seguido pelo nome da função, seguido por parenteses, seguidos por colchetes.

O nome segue as regras de definiçao de uma variavel(letras, numeros...).

Os parametros opcionais são listados entre parenteses(p1, p2...)

O código a ser executado está listado entre chaves{código}. Ex:
```js
function nome(p1, p2, p3) { // código }
```
Agora vamos falar sobre os formatos, que são esses: declaration, expression e arrow.

A começar pela function DECLARATION:

É a forma classica de declarar funçoes em JS. Ela é elevada(hoisted), ou seja, o JavaScript "move" essa declaraçao para o topo do código, o que permite chama-la antes mesmo de ser declarada. Ex:
```js
saudacao(); 
function saudacao() {
  console.log("Olá, Fulano!");
}
```

function EXPRESSION

Aqui, a funçao é atribuida a uma variavel. Ela não é elevada, então precisa ser declarada antes de ser  usada. Ex:

```js
saudacao = function() {
  console.log("Olá, Fulano!");
};

saudacao();
```

function ARROW:


É uma forma mais curta e moderna(ES6+) de escrever funçoes. Ela não tem seu proprio this, herdando o this do escopo onde está. Ex:


somar = (a, b) => a + b;


dobro = (n) => {
   const resultado = n * 2;
  return resultado;
};

console.log(somar(3, 4)); 
console.log(dobro(5));    











