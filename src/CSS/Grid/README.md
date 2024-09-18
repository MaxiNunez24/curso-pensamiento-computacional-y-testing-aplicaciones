# Introducción a CSS Grid

## 1. ¿Qué es CSS Grid?
CSS Grid es un sistema de diseño bidimensional que permite organizar elementos en filas y columnas. Es una herramienta poderosa que facilita la creación de layouts complejos sin tener que depender tanto de `float`, `position`, o incluso `Flexbox`. Con Grid, podemos manejar el diseño de una página tanto horizontal como verticalmente.

## 2. Historia
CSS Grid fue introducido en marzo de 2017 como parte de CSS3, revolucionando la forma en que los desarrolladores crean layouts en la web. Antes de su llegada, los diseñadores tenían que combinar varias técnicas (como tablas, `float` y Flexbox) para lograr diseños responsivos y complejos. CSS Grid simplificó este proceso, haciéndolo más intuitivo y eficiente.

## 3. Sintaxis básica de CSS Grid

```css
.container {
  display: grid; /* Define el contenedor como un grid */
  grid-template-columns: 200px 200px 200px; /* Define tres columnas de 200px cada una */
  grid-template-rows: auto; /* Define una altura automática para las filas */
  grid-gap: 10px; /* Define un espacio entre los elementos del grid */
}
```

- **display: grid**: Define el contenedor como una "rejilla" donde los elementos hijos se organizan en filas y columnas.
- **grid-template-columns**: Define el número y el tamaño de las columnas.
- **grid-template-rows**: Define el número y el tamaño de las filas.
- **grid-gap**: Define el espacio entre las filas y las columnas.

## 4. Ejemplo básico

```html
<div class="grid-container">
  <div class="item1">1</div>
  <div class="item2">2</div>
  <div class="item3">3</div>
  <div class="item4">4</div>
</div>
```

```css
.grid-container {
  display: grid;
  grid-template-columns: repeat(2, 1fr); /* Crea 2 columnas iguales */
  grid-template-rows: 100px 100px; /* Crea 2 filas de 100px cada una */
  grid-gap: 10px; /* Añade un espacio de 10px entre las filas y columnas */
}
```

Este código genera un layout de 2x2 con un espacio de 10px entre las celdas.

## 5. Propiedades importantes

- **grid-template-areas**: Permite definir áreas del grid con nombres que luego podemos asignar a los elementos.

```css
.grid-container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
}

.header {
  grid-area: header;
}
.sidebar {
  grid-area: sidebar;
}
.main {
  grid-area: main;
}
.footer {
  grid-area: footer;
}
```

- **justify-items** y **align-items**: Alinean los elementos dentro de sus celdas tanto horizontal como verticalmente.
  
  ```css
  .grid-container {
    justify-items: center; /* Centra horizontalmente */
    align-items: center; /* Centra verticalmente */
  }
  ```

- **grid-auto-flow**: Define cómo se colocan los elementos si no se especifica una posición.

## 6. Ejercicios prácticos

### Ejercicio 1: Galería de imágenes

Crea una galería de imágenes que se ajuste al tamaño del navegador usando Grid.

- Crea un contenedor con `display: grid`.
- Utiliza `grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));` para que las imágenes se adapten automáticamente.
- Aplica `grid-gap` para añadir espacio entre las imágenes.

### Ejercicio 2: Layout de página web

Crea un layout para una página web con las siguientes secciones: encabezado, barra lateral, contenido principal, y pie de página. Usa `grid-template-areas` para organizar las áreas.

```css
.grid-container {
  display: grid;
  grid-template-columns: 1fr 3fr;
  grid-template-rows: auto 1fr auto;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
}
```

### Ejercicio 3: Tablero de ajedrez

Utiliza CSS Grid para crear un tablero de ajedrez con 8x8 casillas, alternando los colores de las celdas.

```css
.board {
  display: grid;
  grid-template-columns: repeat(8, 50px);
  grid-template-rows: repeat(8, 50px);
}

.cell:nth-child(odd) {
  background-color: black;
}

.cell:nth-child(even) {
  background-color: white;
}
```

## 7. Recursos adicionales
- [CSS Grid en MDN](https://developer.mozilla.org/es/docs/Web/CSS/CSS_Grid_Layout)
- [CSS Tricks: Guía completa de CSS Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)
- [Grid Garden](https://cssgridgarden.com/)

## 8. FAQ

**¿Flexbox o Grid?**  
Ambos tienen usos distintos. Flexbox es ideal para layouts de una dimensión (fila o columna), mientras que Grid es perfecto para layouts bidimensionales.

**¿Cómo se puede hacer que un Grid sea responsivo?**  
Utiliza unidades relativas como `fr`, `auto-fill`, `minmax()`, y `media queries` para que el grid se ajuste al tamaño del navegador.

## 9. Glosario

- **fr**: Unidad flexible para distribuir el espacio disponible entre las columnas o filas de un grid. (Fracción)
- **Grid Template Areas**: Un sistema que asigna nombres a las áreas del grid para facilitar su organización.
- **Grid Gap**: El espacio entre las filas y las columnas de un grid.
