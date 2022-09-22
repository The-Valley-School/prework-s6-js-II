## EJERCICIO 1

```js
/* 
	a) Definir un objeto Persona con las propiedades nombre, apellido, edad y sexo.
	b) Modificar cada una de las propiedades sin volver a definirlo
*/

// A
let persona = {
	nombre: "Eduardo",
	apellido: "Cuadrado",
	edad: 31,
	sexo: "Hombre"
};

console.log(persona);

// B
persona.nombre = "Pepito";
persona.apellido = "García";
persona.edad = 45;
persona.sexo = "Hombre";

console.log(marcaZapatilla);
```

## EJERCICIO 2

```js
/* 
	a) Crear un objeto coche con las propiedades marca, modelo y año. 
		 Metiendo los datos que queramos.
	b) Si el coche tiene más de 25 mostrar por consola un mensaje de este estilo:
		"El seat 600 es un clásido de 1960"
 	c) Si el coche tiene menos de 25 mostrar por consola un mensaje de este estilo:
		"El ford focus del 2010 no es un clásico" 
*/

// A
let coche = {
	marca: "Fiat",
	modelo: "500",
	ano: 2020
};

console.log(coche);

// B y C
if ( (2022 - coche.ano) > 25 ) {
	console.log("El " + coche.marca + " " + coche.modelo + " es un clásico de " + coche.ano);
} else {
	console.log("El " + coche.marca + " " + coche.modelo + " del " + coche.ano + " no es un clásico");
} 
```

## EJERCICIO 3

```js
/* 
	Tengo 2 arrays:
		Propiedades -> ["marca", "modelo", "ano"]
		Valores -> ["Fiat", "500", 2020]
	
	Crear con un bucle for un objeto coche, que tenga las propiedades del primer 
	array y asociados los valores del segundo

*/

let propiedades = ["marca", "modelo", "ano"];
let valores = ["Fiat", "500", 2020];
let coche = new Object();

for (let i=0; i < propiedades.length; i++){
  coche[propiedades[i]] = valores[i];
}

console.log(coche);

```
