# Lab: Funciones básicas con Objetos y Arrays en JavaScript

Este laboratorio te ayudará a practicar la creación de funciones que manipulen y trabajen con **objetos** y **arrays** de forma independiente. Aprenderás a escribir funciones que operen sobre datos simples almacenados en estos tipos de estructuras.

## Requisitos previos

Antes de comenzar este laboratorio, asegúrate de tener los siguientes conocimientos:

- Cómo declarar y utilizar variables
- Conceptos básicos de arrays y objetos
- Cómo escribir y utilizar funciones en JavaScript

---

## Parte 1: Funciones básicas con Objetos

En esta sección, escribirás funciones que interactúan con objetos.

---

### Ejercicio 1: Crear y mostrar un objeto

En este ejercicio, vas a crear una función que tome valores como parámetros y cree un objeto.

### Instrucciones

1. Crea una función llamada `crearPersona` que reciba tres parámetros: `nombre`, `edad`, y `ocupacion`.
2. Dentro de la función, crea un objeto que tenga esas tres propiedades: `nombre`, `edad`, y `ocupacion`.
3. Retorna el objeto creado desde la función.
4. Llama a la función y muestra el objeto resultante en la consola.

### Ejemplo de código

```javascript
function crearPersona(nombre, edad, ocupacion) {
  const persona = {
    nombre: nombre,
    edad: edad,
    ocupacion: ocupacion,
  };
  return persona;
}

const persona1 = crearPersona("Ana", 30, "Ingeniera");
console.log(persona1);
```

### Ejemplo de salida

```
{ nombre: 'Ana', edad: 30, ocupacion: 'Ingeniera' }
```

---

### Ejercicio 2: Modificar una propiedad de un objeto

En este ejercicio, vas a escribir una función que modifique una propiedad de un objeto.

### Instrucciones

1. Crea una función llamada `cambiarEdad` que reciba dos parámetros: un objeto `persona` y un número `nuevaEdad`.
2. Dentro de la función, actualiza la propiedad `edad` del objeto `persona` con el valor de `nuevaEdad`.
3. Muestra el objeto modificado en la consola.

### Ejemplo de código

```javascript
function cambiarEdad(persona, nuevaEdad) {
  persona.edad = nuevaEdad;
}

const persona2 = { nombre: "Luis", edad: 25, ocupacion: "Doctor" };
cambiarEdad(persona2, 28);
console.log(persona2);
```

### Ejemplo de salida

```
{ nombre: 'Luis', edad: 28, ocupacion: 'Doctor' }
```

---

### Ejercicio 3: Obtener una propiedad de un objeto

En este ejercicio, escribirás una función que devuelva el valor de una propiedad de un objeto.

### Instrucciones

1. Crea una función llamada `obtenerOcupacion` que reciba como parámetro un objeto `persona`.
2. La función debe devolver el valor de la propiedad `ocupacion`.
3. Llama a la función y muestra el valor de la ocupación en la consola.

### Ejemplo de código

```javascript
function obtenerOcupacion(persona) {
  return persona.ocupacion;
}

const persona3 = { nombre: "Carlos", edad: 40, ocupacion: "Profesor" };
const ocupacion = obtenerOcupacion(persona3);
console.log(ocupacion);
```

### Ejemplo de salida

```
Profesor
```

---

## Parte 2: Funciones básicas con Arrays

En esta sección, escribirás funciones que trabajen con arrays de forma básica.

---

### Ejercicio 4: Agregar un elemento a un array

En este ejercicio, crearás una función que agregue un nuevo elemento al final de un array.

### Instrucciones

1. Crea una función llamada `agregarElemento` que reciba dos parámetros: un array `elementos` y un nuevo valor `nuevoElemento`.
2. Dentro de la función, agrega el `nuevoElemento` al final del array `elementos` usando el método `push()`.
3. Muestra el array modificado en la consola.

### Ejemplo de código

```javascript
function agregarElemento(elementos, nuevoElemento) {
  elementos.push(nuevoElemento);
}

const frutas = ["manzana", "banana", "naranja"];
agregarElemento(frutas, "uva");
console.log(frutas);
```

### Ejemplo de salida

```
["manzana", "banana", "naranja", "uva"]
```

---

### Ejercicio 5: Remover el primer elemento de un array

En este ejercicio, escribirás una función que elimine el primer elemento de un array.

### Instrucciones

1. Crea una función llamada `removerPrimerElemento` que reciba un array `elementos` como parámetro.
2. Dentro de la función, utiliza el método `shift()` para eliminar el primer elemento del array.
3. Muestra el array modificado en la consola.

### Ejemplo de código

```javascript
function removerPrimerElemento(elementos) {
  elementos.shift();
}

const colores = ["rojo", "azul", "verde"];
removerPrimerElemento(colores);
console.log(colores);
```

### Ejemplo de salida

```
["azul", "verde"]
```

---

### Ejercicio 6: Obtener el tamaño de un array

En este ejercicio, escribirás una función que devuelva el número de elementos en un array.

### Instrucciones

1. Crea una función llamada `obtenerTamañoArray` que reciba un array `elementos` como parámetro.
2. La función debe devolver el tamaño del array utilizando la propiedad `length`.
3. Muestra el tamaño del array en la consola.

### Ejemplo de código

```javascript
function obtenerTamañoArray(elementos) {
  return elementos.length;
}

const animales = ["perro", "gato", "conejo"];
const tamaño = obtenerTamañoArray(animales);
console.log(tamaño);
```

### Ejemplo de salida

```
3
```

---

### Ejercicio 7: Encontrar un elemento en un array

En este ejercicio, escribirás una función que verifique si un array contiene un elemento específico.

### Instrucciones

1. Crea una función llamada `encontrarElemento` que reciba dos parámetros: un array `elementos` y un valor `elementoBuscado`.
2. Utiliza el método `includes()` para verificar si `elementoBuscado` está presente en el array.
3. La función debe devolver `true` si el elemento se encuentra en el array y `false` en caso contrario.
4. Muestra el resultado en la consola.

### Ejemplo de código

```javascript
function encontrarElemento(elementos, elementoBuscado) {
  return elementos.includes(elementoBuscado);
}

const numeros = [1, 2, 3, 4, 5];
const encontrado = encontrarElemento(numeros, 3);
console.log(encontrado);
```

### Ejemplo de salida

```
true
```

---

## Notas adicionales

- Asegúrate de probar cada función con diferentes valores para verificar que tu código funcione correctamente.
- Usa `console.log()` para ver los resultados de tus pruebas y depurar tu código si es necesario.
- Si algo no funciona como esperabas, revisa la lógica de las funciones y cómo estás manipulando los objetos y arrays.

¡Disfruta practicando con funciones, objetos y arrays!
