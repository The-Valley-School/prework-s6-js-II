A la hora de trabajar en JS, muchas veces nos encontraremos ante la necesidad de realizar tareas repetitivas. Para optimizar este proceso podemos hacer uso de los bucles que nos permiten de una manera rápida, realizar una tarea **n** veces, pudiendo ejecutar un trozo de código tantas veces como queramos sin tener que duplicar o triplicar esas lineas.

A lo largo del vídeo vamos a ver 2 tipos de bucles, FOR , WHILE y DO WHILE

## BUCLE FOR

El bucle FOR nos va a permitir repetir un trozo de código el número de veces que le digamos.

La sintaxis para trabajar con bucles FOR es la siguiente

```js
for ( EXPRESION INICIAL; CONDICION; EXPRESION FINAL){
	//Sentencia que se repite 
}
```

- Expresión inicial:  Expresión o declaración de variable. Suele ser para inicializar un contador.
- Condición: Expresión que usamos para la continuidad del bucle, mientras sea verdadera sigo iterando
- Expresión final: Expresión evaluada tras cada iteración. Suelen ser incrementos o decrementos.

Posiblemente todavía te suene a chino, pero con un ejemplo seguro que lo entendemos mejor. Vamos a imprimir por consola los números del 1 al 10.

```js
for (let i = 0; i <= 10; i++){
	 console.log(i);
} 
```

Analizamos detalladamente:

- Nuestra expresión inicial es **let i = 0** , estamos declarando una variable **i**  que vale 0
- Con la condición **i ≤ 10** indicamos que vamos a ejecutar el bucle hasta que la variable **i** valga 10. Cada vez que se itere en el bucle se validará esta condición
- La expresión final **i++** nos indica que cuando se termine una iteración se le añadirá un +1 a nuestra variable **i.**
- El bucle terminará cuando **i** sea mayor que 10, según la condición propuesta.

Si quisiésemos contar hacia atrás podríamos hacerlo:

```js
for (let i = 10; i = 0; i--){
	 console.log(i);
} 
```

En este caso, iríamos reduciendo la variable **i** que utilizamos como índice para contar hacia atrás.

Al poner en la expresión final **i—** estamos indicamos que estamos reduciendo 1 en cada iteración al valor de **i.**

Vamos a realizar otro ejemplo para seguir trabajando con los bucles FOR. En esta ocasión vamos a crear la tabla de multiplicar del 7 y mostrar los resultados por pantalla.

```js
for (let i = 0; i <= 10; i++){
	 console.log(7 * i);
} 
```

Estamos recorriendo el bucle 11 veces, desde que **i = 0,** hasta que **i = 10**. En cada iteración estamos multiplicando el 7 y aprovechando el valor de **i** para ir haciendo la tabla de multiplicar.

Por último, vamos a hacer un ejercicio con textos. La propiedad **.length** nos devuelve el número total de caracteres dentro de un string, así que vamos a recorrer uno y lanzar por consola cada una de las letras. Para conseguir un caracter específico de una cadena de texto debemos de seleccionar la variable junto con el índice del caracter que queremos de tal forma → **texto[i]**

```js
let palabra = "Pepito";
let primeraLetraPalabra = palabra[0] 
console.log(primeraLetraPalabra) // Pinta la letra P, en programación se empieza a contar desde el 0
```

Sabiendo como seleccionar un caracter vamos a proceder a realizar la iteración 

```js
let palabra = "Pepito";

for (let i = 0; i <= palabra.length; i++){
	 console.log(palabra[i]);
} 
```
