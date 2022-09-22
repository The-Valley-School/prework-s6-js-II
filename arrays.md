## DEFINICIÓN DE ARRAYS

Tras ver los tipos de datos primitivos, vamos ahora a ver otro tipo de datos, que son los arrays. A lo largo del master profundizaremos más sobre ellos pero de momento vamos a ver qué son y cómo trabajar con ellos. 

Un array, es conjunto de datos, un listado de datos (strings, numbers...) que irán entre corchetes y separados por comas. La sintaxis es la siguiente:

```js
[ ELEMENTO1, ELEMENTO2, ..., ELEMENTON]
```

Podemos tener tanto listados de todo tipo: numéricos, de strings, mixtos…

```js
let numerosPremiados = [3, 5, 43, 18, 27];
let listaCompra = [ "Manzanas", "Peras", "Carne", "Papel de cocina"];
let varios = [3, "Manzanas", null, 18, true];
```

## ACCEDER A LOS ELEMENTOS DE UN ARRAY

Para acceder a los elementos de un array tenemos que entender el mismo como un listado, que empieza en 0. Al igual que cuando hemos trabajado con los caracteres de un string.

```js
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];
let personaje = familiaSimpson[0];
console.log(personaje); //Mostrará por consola a Homer
```

Homer es la **posición 0** del array, Marge sería la **posición 4.**

## PROPIEDAD LENGTH

Para conocer el número de elementos de un array se puede consultar con la propiedad length.

```js
familiaSimpson.length;
```

Vamos a aprovechar y ya que sabemos trabajar con bucles, para mostrar por consola todos los elementos del array.

```js
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];
for ( let i = 0; i < familiaSimpson.length; i++){
    console.log(familiaSimpson[i]);
}
```

## MANIPULAR EL ARRAY

Podemos también modificar un elemento concreto del array si indicamos su posición.

```js
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];

familiaSimpson[1] = "Mou"; //Estamos cambiando a Bart por Mou
console.log(familiaSimpson);
```

## POP Y PUSH

Pop y push son dos métodos con los cuales podemos eliminar y añadir elemento al final del array.

POP (eliminando elementos)

```js
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];

familiaSimpson.pop();
console.log(familiaSimpson); //Mostrará el listado sin Maggie

familiaSimpson.pop();
console.log(familiaSimpson); //Mostrará el listado sin Maggie y sin Marge
```

PUSH (añadiendo elementos)

```js
let familiaSimpson = [ "Homer", "Bart", "Lisa", "Marge", "Maggie" ];

familiaSimpson.push("Bola de Nieve");
console.log(familiaSimpson); //Mostrará el listado añadiendo al final a Bola de Nieve

familiaSimpson.pop("Ayudante de Santa Claus", "Abe");
console.log(familiaSimpson); //Mostrará el listado añadiendo al final a Ayudante de Santa Claus y a Abe
```
