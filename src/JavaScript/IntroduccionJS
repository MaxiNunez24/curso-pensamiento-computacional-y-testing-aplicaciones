**¡Bienvenidos a la introducción de JavaScript!** Hoy vamos a ver cómo este lenguaje se usa para dar vida a nuestras páginas web. Para esto, vamos a ver conceptos básicos, algunos ejemplos prácticos y cómo JavaScript interactúa con HTML.

---

### Parte 1: Introducción y Estructura de JavaScript en HTML (16:00 - 16:30)

**1. ¿Qué es JavaScript?**
   - JavaScript es un lenguaje de programación que permite agregar dinamismo a las páginas web, como botones interactivos, animaciones, validaciones de formularios, entre muchas otras cosas.

**2. Colocación de JavaScript en HTML**
   - Hay dos formas de agregar JavaScript en HTML:
     - **Directamente en el archivo HTML** usando una etiqueta `<script>`.
     - **Vinculando un archivo externo** usando `<script src="ruta-del-archivo.js"></script>`, que es más organizado cuando tenemos mucho código.

**Ejemplo básico:**

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primera página con JS</title>
</head>
<body>
    <h1>Bienvenidos a mi página</h1>
    <button onclick="saludar()">Haz clic aquí</button>

    <script>
        function saludar() {
            alert("¡Hola a todos! Esta es una prueba de JavaScript en HTML.");
        }
    </script>
</body>
</html>
```

**Explicación**:
   - Cuando el usuario haga clic en el botón, llamará a la función `saludar`, que mostrará un mensaje con `alert()`.

**Preguntas comunes:**
   - **¿Puedo poner el código JavaScript en el `<head>`?** Sí, pero es más común ponerlo justo antes del cierre de `</body>` para mejorar el rendimiento.
   - **¿Es necesario aprender HTML para usar JavaScript?** Conocer HTML ayuda muchísimo porque JavaScript interactúa con los elementos HTML.

---

### Parte 2: Variables, Operadores y Tipos de Datos (16:30 - 17:10)

**1. Variables en JavaScript**
   - Para almacenar valores en JavaScript, usamos variables, y existen tres maneras de declararlas:
     - `let`: para valores que pueden cambiar.
     - `const`: para valores constantes que no cambiarán.
     - `var`: antigua forma de declarar variables (usaremos mejor `let` y `const`).

**Ejemplo:**

```javascript
let nombre = "Juan";
const edad = 20;
console.log(nombre, edad);
```

**2. Tipos de datos y Operadores básicos**
   - Tipos de datos comunes: números (`5`), cadenas de texto (`"Hola"`), booleanos (`true` o `false`).
   - Operadores comunes: `+`, `-`, `*`, `/` para aritmética; `==`, `===`, `<`, `>` para comparación.

**Ejercicio práctico:**
   - Declaremos dos variables: `nombre` y `edad`. Mostremos un mensaje personalizado en la consola usando `console.log()`.

**Posibles preguntas:**
   - **¿Por qué a veces uso `let` y otras `const`?** `const` se usa para valores que no cambian, como una constante; `let` es para valores que pueden cambiar.
   - **¿Por qué `var` ya no se usa tanto?** `let` y `const` tienen un mejor manejo en cuanto al alcance (scope) del código.

**[Recreo de 15 minutos: 17:10 - 17:25]**

---

### Parte 3: Control de Flujo (17:25 - 18:05)

**1. Estructuras de control: `if`, `else`, y `else if`**
   - Nos ayudan a tomar decisiones en el código.
   - Ejemplo simple:

```javascript
let edad = 18;
if (edad >= 18) {
    console.log("Eres mayor de edad");
} else {
    console.log("Eres menor de edad");
}
```

**2. Ciclos: `for` y `while`**
   - Los usamos para repetir acciones.
   - Ejemplo con `for`:

```javascript
for (let i = 0; i < 5; i++) {
    console.log("Este es el número " + i);
}
```

**Práctica guiada:**
   - Creamos un contador que muestra los números del 1 al 10.
   - Hacemos que el usuario ingrese su edad y respondemos si es mayor o menor de edad usando `if` y `prompt()`.

**Posibles preguntas:**
   - **¿Puedo combinar `if` y `for`?** Sí, las estructuras de control y los ciclos se pueden combinar según las necesidades del programa.
   - **¿Qué pasa si escribo `if` sin `else`?** No pasa nada; `else` es opcional y se usa solo si tienes otra acción para cuando la condición de `if` es falsa.

---

### Parte 4: Funciones en JavaScript (18:05 - 18:45)

**1. ¿Qué es una función?**
   - Una función es un bloque de código que realiza una tarea específica y que puedes reutilizar en diferentes partes de tu programa.

**Ejemplo básico:**

```javascript
function saludo(nombre) {
    return "Hola, " + nombre + "!";
}
console.log(saludo("Juan"));
```

**2. Funciones que interactúan con HTML**
   - Ejemplo de cómo crear una función que cambia el texto de un párrafo al hacer clic en un botón:

```html
<p id="miTexto">Texto inicial</p>
<button onclick="cambiarTexto()">Cambiar texto</button>

<script>
    function cambiarTexto() {
        document.getElementById("miTexto").innerHTML = "¡Texto cambiado!";
    }
</script>
```

**Práctica:**
   - Hacemos un formulario en HTML con un campo para el nombre y un botón. Cuando el usuario lo envía, mostramos un mensaje personalizado usando una función JavaScript.

**Preguntas comunes:**
   - **¿Puedo llamar a una función desde otro archivo JS?** Sí, pero debes vincular el archivo en el HTML usando `<script src="nombre-del-archivo.js"></script>`.
   - **¿Qué pasa si llamo una función antes de declararla?** Depende de cómo esté escrita la función. Las `function` regulares pueden “subir” (hoisting), pero las funciones de flecha (que veremos después) no se comportan igual.

---

### Cierre y Repaso (18:45 - 19:10)

1. **Repaso:** Recordamos conceptos clave: ¿qué es JavaScript?, colocación en HTML, variables, operadores, control de flujo, y funciones.
2. **Pregunta abierta:** ¿Para qué piensan que podrían usar JavaScript en sus proyectos? 
3. **Mini reto:** Les dejo el siguiente desafío: en su tiempo libre, intenten hacer que aparezca una alerta con su nombre al abrir la página.
