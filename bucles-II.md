## BUCLE WHILE

El bucle WHILE nos permite iterar un trozo de código mientras se cumpla una condición. 

La sintaxis es la siguiente:

```js
while (CONDICION) {
	// sentencia que se repite
}
```

El bucle WHILE se seguirá repitiendo mientras se cumpla la condición. Esta condición se evalúa al iniciar cada iteración. Vamos a ver un ejemplo:

```js
let n = 0;

while (n <= 3){
    console.log ("La variable n vale: " + n );
    n++;
}
```

En cada iteración vamos aumentando el valor de n. El bucle se repetirá hasta que n valga 3.

## BUCLE DO…WHILE

El bucle DO..WHILE nos permite también iterar un trozo de código mientras se cumpla una condición. La diferencia con el bucle WHILE es que la comprobación se realiza al finalizar la iteración por lo que como mínimo siempre va a pasar una vez por el bucle. La sintaxis es la siguiente:

```js
do {
   //sentencia que se repite
} while(CONDICION);
```

En cada iteración vamos aumentando el valor de a, al igual que en el WHILE, hasta que se cumpla la condición para salir del bucle.

```js
let a = 0;

do {
    console.log ("La variable a vale: " + a );
    a++;
} while (a <= 3);
```
