# Introducción a JavaScript

## ¿Qué es JavaScript?
JavaScript es un lenguaje de programación interpretado, orientado a objetos y dinámico. Es uno de los lenguajes más populares y se utiliza principalmente para el desarrollo web, permitiendo crear páginas web interactivas. Se dice que es el "lenguaje de la web".

## ¿Dónde se ejecuta JavaScript?
JavaScript se puede ejecutar en cualquier navegador web moderno. También se puede ejecutar en el servidor utilizando Node.js. En esta clase, nos centraremos en JavaScript en el navegador.

## Primeros pasos con JavaScript en el navegador
Puedes empezar a programar en JavaScript directamente desde la consola del navegador. Para abrir la consola:
1. Abre tu navegador (Chrome, Firefox, etc.).
2. Abre una página en blanco buscando "`about:blank`" en la barra de direcciones.
3. Haz clic derecho en cualquier parte de la página y selecciona "`Inspeccionar`" o "`Inspect`".
4. Ve a la pestaña "`Consola`" o "`Console`".

## Tipos de datos en JavaScript
JavaScript tiene varios tipos de datos básicos:
- **Number**: `42`, `3.14` (Números) -> se utilizan para almacenar números
- **String**: `"Hola, mundo!"` (Cadena de Texto) -> se utilizan para almacenar texto
- **Boolean**: `true`, `false` (Verdadero o falso) -> se utilizan para tomar decisiones
- **Null**: `null` (Valor nulo) -> representa la ausencia de valor
- **Undefined**: `undefined` (Valor no definido) -> representa una variable que no ha sido asignada

## Variables
Puedes declarar variables (también llamadas "enlaces") usando `var`, `let` o `const`.

```javascript
var nombre = "Juan"; // No se recomienda usar var, más adelante veremos el por qué
let edad = 30; // Se puede reasignar, es preferible usar let a var
const PI = 3.14; // No se puede reasignar
```

## Operadores
### Aritméticos
```javascript
let suma = 5 + 3; // 8
let resta = 5 - 3; // 2
let multiplicacion = 5 * 3; // 15
let division = 6 / 3; // 2
let modulo = 5 % 3; // 2 (resto de la división)
```

### Comparación
```javascript
// Variables
let a = 5;
let b = 10;
// Operadores de comparación
console.log(a == b); // false, porque 5 no es igual a 10
console.log(a != b); // true, porque 5 no es diferente de 10
console.log(a === b); // false, porque 5 no es estrictamente igual a 10
console.log(a !== b); // true, porque 5 no es estrictamente diferente de 10
console.log(a < b); // true, porque 5 es menor que 10
console.log(a > b); // false, porque 5 no es mayor que 10
console.log(a <= b); // true, porque 5 es menor o igual a 10
console.log(a >= b); // false, porque 5 no es mayor o igual a 10
```

### Lógicos
```javascript
// Variables
let x = true;
let y = false;

// Operadores lógicos
console.log(x && y); // false, porque true y false es false
console.log(x || y); // true, porque true o false es true
console.log(!x); // false, porque la negación de true es false
console.log(!y); // true, porque la negación de false es true
```

## Estructuras de datos
### Arreglos
```javascript
// Declaración de un arreglo
let frutas = ["manzana", "banana", "naranja"]; 

// Acceder a un elemento del arreglo
console.log(frutas[0]); // manzana
console.log(frutas[1]); // banana
console.log(frutas[2]); // naranja
```

### Objetos
```javascript
// Declaración de un objeto
let persona = { // Un objeto tiene propiedades
    nombre: "Juan", // Propiedad: valor
    edad: 30,
    casado: false
};

// Acceder a una propiedad del objeto
console.log(persona.nombre); // Juan
console.log(persona.edad); // 30
console.log(persona.casado); // false
```

## Operadores de incremento y decremento
```javascript
let i = 5;
// Post-incremento
console.log(i++); // 5, imprime i y luego incrementa -> es equivalente a i = i + 1
console.log(i); // 6
// Pre-incremento
console.log(++i); // 7, incrementa i y luego imprime -> es equivalente a i = i + 1
console.log(i); // 7
```

## Estructuras de control
### Condicionales
```javascript
if (edad > 18) { // Si la edad es mayor a 18 (condición)
    console.log("Eres mayor de edad"); // Si se cumple la condición -> imprime en la consola "Eres mayor de edad"
} else {
    console.log("Eres menor de edad"); // Si no se cumple la condición -> imprime en la consola "Eres menor de edad"
}
```

### Bucles
#### Bucle `for`
```javascript
for (let i = 0; i < 5; i++) { // Inicialización; condición; incremento
    console.log(i); // Imprime el valor de i en la consola
}
```

#### Bucle `while`
```javascript
let i = 0;
while (i < 5) { // Mientras i sea menor a 5
    console.log(i); // Imprime el valor de i en la consola
    i++; // Incrementa i -> evita un bucle infinito
}
```

## Funciones
Las funciones son bloques de código reutilizables.
Un ejemplo que venimos usando hasta ahora: `console.log("Hola, Mundo!")`. -> `console.log` es una función que imprime lo que le pasamos como argumento en la consola.

```javascript
function saludar(nombre) { // Declaración de una función llamada "saludar" con un parámetro "nombre"
    return "Hola, " + nombre; // Devuelve un saludo con el nombre pasado como argumento
} 


console.log(saludar("Juan")); // Llama a la función "saludar" con el argumento "Juan"
// Imprime en la consola "Hola, Juan"

``` 
### Cuál es la diferencia entre argumento y parámetro?
- **Parámetro**: es el nombre que se le da a la variable que recibe la función
- **Argumento**: es el valor que se le pasa a la función

## Ejercicios
1. **Hola, Mundo!**: Escribe un programa que imprima "Hola, Mundo!" en la consola.
2. **Suma de dos números**: Escribe una función que reciba dos números y devuelva su suma.
3. **Número par o impar**: Escribe un programa que determine si un número es par o impar.
4. **Contar hasta 10**: Escribe un bucle que cuente del 1 al 10 y lo imprima en la consola.
5. **Arreglo de nombres**: Crea un arreglo con nombres de personas y escribe un programa que imprima cada nombre en la consola.