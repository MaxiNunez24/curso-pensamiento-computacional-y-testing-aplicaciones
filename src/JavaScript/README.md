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

## Comentarios
Los comentarios son útiles para explicar el código y hacerlo más legible. En JavaScript, los comentarios de una sola línea comienzan con `//` y los comentarios de varias líneas comienzan con `/*` y terminan con `*/`.

```javascript
// Este es un comentario de una sola línea

/*
Este es un comentario
de varias líneas
*/
```

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
let a = 5
let b = 10
// Operadores de comparación
a == b; // false, porque 5 no es igual a 10
a != b // true, porque 5 no es diferente de 10
a === b // false, porque 5 no es estrictamente igual a 10
a !== b // true, porque 5 no es estrictamente diferente de 10
a < b // true, porque 5 es menor que 10
a > b // false, porque 5 no es mayor que 10
a <= b // true, porque 5 es menor o igual a 10
a >= b // false, porque 5 no es mayor o igual a 10
```

### Lógicos
```javascript
// Variables
let x = true;
let y = false;

// Operadores lógicos
x && y // false, porque true y false es false
x || y // true, porque true o false es true
!x // false, porque la negación de true es false
!y // true, porque la negación de false es true
```

### Asignación
```javascript
let a = 5;
a += 3 // a = a + 3 -> 8
a -= 3 // a = a - 3 -> 5
a *= 3 // a = a * 3 -> 15
a /= 3 // a = a / 3 -> 5
a %= 3 // a = a % 3 -> 2
```

## Diferencia entre Expresión y Sentencia
- **Expresión**: es una combinación de valores, variables y operadores que se evalúa para producir un valor.
- **Sentencia**: es una instrucción que realiza una acción. Por ejemplo, una sentencia de asignación asigna un valor a una variable. No devuelve un valor.

```javascript
// Expresión
5 + 3; // es una expresión que se evalúa a 8 -> devuelve 8

// Sentencia
let y = 5; // es una sentencia que asigna el valor 5 a la variable y -> devuelve undefined porque no hay nada que devolver

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
Un ejemplo que venimos usando hasta ahora: `console.log("Hola, Mundo!")`. 
`console.log` es una función que imprime lo que le pasamos como argumento en la consola.

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


## Strings
```javascript  
let nombre = "Juan"; // Declaración de una variable de tipo string
let apellido = "Pérez";
let nombreCompleto = nombre + " " + apellido; // Concatenación de strings
console.log(nombreCompleto); // Juan Pérez
```

## Funciones de Strings
```javascript
let cadena = "Hola, Mundo!";
console.log(cadena.length); // 12, longitud de la cadena
console.log(cadena.toUpperCase()); // HOLA, MUNDO!, convierte la cadena a mayúsculas
console.log(cadena.toLowerCase()); // hola, mundo!, convierte la cadena a minúsculas
console.log(cadena.charAt(0)); // H, devuelve el carácter en la posición 0
console.log(cadena.indexOf("Mundo")); // 6, devuelve la posición de la primera ocurrencia de "Mundo"
console.log(cadena.slice(0, 4)); // Hola, devuelve una subcadena desde la posición 0 hasta la 4
console.log(cadena.split(",")); // ["Hola", " Mundo!"], divide la cadena en un arreglo
console.log(cadena.reverse()); // !odnuM ,aloH, invierte la cadena
console.log(cadena.replace("Mundo", "Amigo")); // Hola, Amigo!, reemplaza "Mundo" por "Amigo"
console.log(cadena.includes("Hola")); // true, devuelve true si la cadena contiene "Hola"
console.log(cadena.startsWith("Hola")); // true, devuelve true si la cadena comienza con "Hola"
console.log(cadena.endsWith("Mundo!")); // true, devuelve true si la cadena termina con "Mundo!"
console.log(cadena.trim()); // Hola, Mundo!, elimina los espacios en blanco al principio y al final
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

## Ejercicios
1. **Hola, Mundo!**: Escribe un programa que imprima "Hola, Mundo!" en la consola.
    <details><summary>Ver posible posible respuesta</summary>
    
    ```javascript
    console.log("Hola, Mundo!");
    ```
    </details>

2. **Saludar a alguien**: Escribe una función que reciba un nombre y devuelva un saludo.
    <details><summary>Ver posible respuesta</summary>

    ```javascript
    function saludar(nombre) {
        return "Hola, " + nombre;
    }
    console.log(saludar("Juan"));
    ```
        
    </details>

3. **Número par o impar**: Escribe un programa que determine si un número es par o impar.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    let numero = 5; // También se puede hacer una función que reciba un número como argumento

    if (numero % 2 === 0) {
        console.log("El número es par");
    } else {
        console.log("El número es impar");
    }
    ```
    </details>

4. **Suma de dos números**: Escribe una función que reciba dos números y devuelva su suma. 
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function sumar(a, b) {
        return a + b;
    }

    console.log(sumar(5, 3));
    ```
    </details>

5. **Contar hasta 10**: Escribe un bucle que cuente del 1 al 10 y lo imprima en la consola.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    for (let i = 1; i <= 10; i++) {
        console.log(i);
    }
    ```
    </details>

5. **Números primos**: Escribe un programa que determine si un número es primo. (Un número primo es aquel que solo es divisible por 1 y por sí mismo).
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    let numero = 7; // También se puede hacer una función que reciba un número como argumento
    let esPrimo = true, i = 2;
    while (i < numero && esPrimo) {
        if (numero % i === 0) esPrimo = false;
        i++;
    }

    if (esPrimo) {
        console.log("El número es primo");
    } else {
        console.log("El número no es primo");
    }
    ```
    </details>

6. **Arreglo de nombres**: Crea un arreglo con nombres de personas y escribe un programa que imprima cada nombre en la consola.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    let nombres = ["Juan", "María", "Pedro", "Ana"];

    for (let i = 0; i < nombres.length; i++) {
        console.log(nombres[i]);
    }
    ```
    </details>

12. **Máximo de un arreglo**: Escribe una función que reciba un arreglo de números y devuelva el número más grande.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function maximo(arreglo) {
        let max = arreglo[0];
        for (let i = 1; i < arreglo.length; i++) {
            if (arreglo[i] > max) {
                max = arreglo[i];
            }
        }
        return max;
    }

    console.log(maximo([5, 3, 8, 1, 2]));
    ```
    </details>

18. **Promedio de un arreglo**: Escribe una función que calcule el promedio de los números en un arreglo.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function promedio(arreglo) {
        let suma = 0;
        for (let i = 0; i < arreglo.length; i++) {
            suma += arreglo[i];
        }
        return suma / arreglo.length;
    }

    console.log(promedio([5, 3, 8, 1, 2]));
    ```
    </details>

16. **Buscar en un arreglo**: Escribe una función que busque un elemento en un arreglo y devuelva su índice.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function buscar(arreglo, elemento) {
        let i = 0, pos = -1, encontrado = false;
        while (i < arreglo.length && !encontrado) {
            if (arreglo[i] === elemento) {
                encontrado = true;
                pos = i;
            }
            i++;
        }
        return pos;
    }

    console.log(buscar([5, 3, 8, 1, 2], 8));
    ```
    </details>

7. **Objeto de persona**: Crea un objeto con las propiedades "nombre", "apellido", "edad" y "casado" e imprime cada propiedad en la consola.
    <details><summary>Ver posible posible respuesta</summary>
    
    ```javascript
    let persona = {
        nombre: "Juan",
        apellido: "Pérez",
        edad: 30,
        casado: false
    };

    console.log(persona.nombre);
    console.log(persona.apellido);
    console.log(persona.edad);
    console.log(persona.casado);
    ```
    </details>

10. **Revertir una cadena**: Escribe una función que reciba una cadena y devuelva la cadena invertida. Por ejemplo, si la cadena es "hola", la función debería devolver "aloh".
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function invertir(cadena) {
        return cadena.split("").reverse().join(""); // Divide la cadena en un arreglo, invierte el arreglo y lo une en una cadena
        // esto es lo mismo que: cadena.reverse()
    }

    console.log(invertir("hola"));
    ```
    </details>

11. **Contar vocales**: Escribe una función que cuente el número de vocales en una cadena.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function contarVocales(cadena) {
        let vocales = "aeiouAEIOU";
        let contador = 0;
        for (let i = 0; i < cadena.length; i++) {
            if (vocales.includes(cadena[i])) {
                contador++;
            }
        }
        return contador;
    }

    console.log(contarVocales("Hola, Mundo!"));
    ```
    </details>

9. **Factorial de un número**: Escribe una función que calcule el factorial de un número.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function factorial(n) {
        if (n === 1) return 1;
        return n * factorial(n - 1);
    }

    console.log(factorial(5));
    ```
    </details>

14. **Fibonacci**: Escribe una función que genere los primeros n números de la secuencia de Fibonacci.
    <details><summary>Ver posible respuesta</summary>
    
    ```javascript
    function fibonacci(n) {
        fib = [0, 1];
        for (let i = 2; i < n; i++) {
            fib[i] = fib[i - 1] + fib[i - 2];
        }
        return fib;
    }

    console.log(fibonacci(10));
    ```
    </details>


