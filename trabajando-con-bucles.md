Vamos ahora a hacer 3 ejercicios para asentar los conocimientos de bucles. Nos vamos a centrar en el bucle FOR que es el que más utilizaremos a lo largo de nuestros desarrollos.

**EJERCICIO 1**

```js
// Cuenta del 330 al 910

for (let i = 330; i <= 910; i++) {
    console.log(i);
}
```

**EJERCICIO 2**

```js
// Suma todos los números pares del 1 al 1000 (sin incluir el 1000)

let sumador = 0;

for (let i = 1; i < 1000; i++){
    if( i % 2 === 0) {   
        console.log(i);
        sumador += i;
    }
}

console.log(sumador);
```

**EJERCICIO 3**

```js
// Cuenta el número de 'i' que tiene la palabra 'supercalifragilisticoespialidoso’

let palabra = "supercalifragilisticoespialidoso";
let contador = 0;

for (let i=0; i < palabra.length; i++){
    if (palabra[i] === 'i'){
        contador++;
    }
}

console.log(contador);
```
