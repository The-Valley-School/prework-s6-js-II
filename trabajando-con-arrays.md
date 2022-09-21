**EJERCICIO 1**

```js
/*
  Crea un listado con 5 frutas, elimina las dos últimas, 
  añade 3 más y verifica la longitud del array.
*/

let frutas = ["melón", "manzana", "pera", "plátano", "naranja"];

// Eliminamos las dos últimas:
frutas.pop(); // Eliminamos naranja
frutas.pop(); // Eliminamos plátano

// Añadimos tres nuevas:
frutas.push("fresa", "sandía", "kiwi");

console.log(frutas); // Comprobamos el array
console.log(frutas.length) // Verificamos la longitud del array

```

**EJERCICIO 2**

```js
/*
  Crea un array vacío y utilizando un bucle for, itera del 1 al 20 y 
  ve añadiendo esos números al array. El resultado debería ser:
  [1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20]
*/

let listadoNumeros = [];

for ( let i = 1; i <= 20; i++ ) {
	listadoNumeros.push(i);
}

console.log(listadoNumeros) // Comprobamos el array
```

**EJERCICIO 3**

```js
/*
  Teniendo el siguiente array: 
  ["VERDE", "AZUL", "AMARILLO", "NARANJA", "VIOLETA", "MARRON"]

  Usando un bucle genera un array con el núemero de caracteres de cada palabra. 
  El resultado tendría que ser
  [5,4,8,7,7,6]
*/

let colores = ["VERDE", "AZUL", "AMARILLO", "NARANJA", "VIOLETA", "MARRON"];
let letrasColores = [];

for ( i = 0; i < colores.length; i++ ){
	letrasColores.push(colores[i].length);
}

console.log(letrasColores);
```
