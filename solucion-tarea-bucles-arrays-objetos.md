## EJERCICIO 1

```js
/*
	A) Crea una variable con la suma todos los números impares del 300 al 400
	B) Crea un array con todos los números pares, utilizando el bucle 
	del apartado A 
*/

let sumador = 0;
let numerosPares = [];

for (let i = 300; i <= 400; i++){
    if ( i % 2 === 1){
        sumador += i;
    } else {
        numerosPares.push(i);
    }
}

console.log(sumador);
console.log(numerosPares);
```

## EJERCICIO 2

```js
/*
	A) Crea un array con 5 películas que te gusten
	B) Muestra esas 5 películas por consola, usando un bucle for. 
		Las películas tienen que mostrarse de la última posición a la primera.

	Ejemplo de array -> ["E.T.", "Toy Story", "Bichos", "Nemo", "Dori"]
	Resultado por consola:
		Dori
		Nemo
		Bichos
		Toy Story
		E.T.
*/

let peliculas = ["E.T.", "Toy Story", "Bichos", "Nemo", "Dori"];

for (let i = (peliculas.length - 1); i >= 0; i--){
    console.log(peliculas[i]);
}
```

## EJERCICIO 3

```js
/*
	Teniendo el siguiente array: 
	[3, 7, 20, 12, 100, 50, 5, 2, 40]
	
	Usando un bucle genera un array que indique **true** si el número del array
	es mayor que 10 y **false** si es menor o igual
	
	La solución sería el siguiente array :
	[false, false, true, true, true, true, false, false, true]
*/

let peliculas = [3, 7, 20, 12, 100, 50, 5, 2, 40];
let mayor10 = [];

for (let i = 0; i < peliculas.length; i++){
   if ( peliculas[i] > 10 ){
        mayor10[i] = true;
   } else {
        mayor10[i] = false;
   }

}
console.log(mayor10);
```

## EJERCICIO 4

```js
/* 
	A) Crear un objeto cancion con las propiedades titulo, cantante, duracion(en segundos) y genero. 
	Metiendo los datos que queramos.
	Ejemplo: Zapatillas, El canto del loco, 180, pop
	B) Utilizando un swicth con el género, sacar por consola si me gusta o no este tipo 
	de música.
	Generos que debe contemplar el switch: pop, rock, trap, punk
	Si el tipo de canción es rock o trap, el mensaje será "Me gusta la canción XXX (titulo de la canción objeto)"
	Si el tipo de canción es trap o punk, el mensaje será "No me gusta XXX (cantante del objeto canción)"
	Si el género es diferente a esto, el mensaje será "No he escuchado este género"
*/

let cancion = {
    titulo: "Zapatillas",
    cantante: "El canto del loco",
    duracion: 180,
    genero: "pop"
}

switch(cancion.genero){
    case "pop":
        console.log("No me gusta " + cancion.cantante);
        break;
    case "rock":
        console.log("Me gusta la canción " + cancion.titulo);
        break;
    case "trap":
        console.log("Me gusta la canción " + cancion.titulo);
        break;
    case "punk":
        console.log("No me gusta " + cancion.cantante);
        break;
    default:
        console.log("No he escuchado este género");
        break;
}
```
