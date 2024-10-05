[Volver al inicio](../../../README.md)
[Volver a CSS](../README.md) 
# Guía de Introducción a Flexbox

## 1. ¿Qué es Flexbox?

**Flexbox**, o *"Flexible Box Layout"*, es un **modelo de diseño** de CSS que facilita la **distribución de elementos** en un **contenedor**, especialmente cuando se trata de distribuir espacio y **alinear elementos de manera flexible** y eficiente. Es ideal para crear **layouts** que se **adapten** a diferentes tamaños de pantalla y resoluciones.

## 2. Contenedor Flex y Elementos Flex

### 2.1. Definir un Contenedor Flex

Para convertir un contenedor en un **contenedor Flex**, se debe aplicar la propiedad `display: flex;` al elemento padre.

```css
.contenedor {
    display: flex;
}
```

### 2.2. Ejes en Flexbox

- **Eje principal (main axis)**: Es el eje principal a lo largo del cual se distribuyen los elementos flex. Por defecto, es horizontal.
- **Eje transversal (cross axis)**: Es perpendicular al eje principal.

## 3. Propiedades Principales de Flexbox

### 3.1. `justify-content`

Controla cómo se distribuyen los elementos a lo largo del eje principal.

- `flex-start`: Los elementos se alinean al **inicio** del contenedor.
- `flex-end`: Los elementos se alinean al **final** del contenedor.
- `center`: Los elementos se alinean en el **centro** del contenedor.
- `space-between`: Los elementos se **distribuyen uniformemente** con el primer elemento alineado al principio y el último al final.
- `space-around`: Los elementos se **distribuyen uniformemente** con **espacios iguales** alrededor de cada elemento.

```css
.contenedor {
    display: flex;
    justify-content: center;
}
```

### 3.2. `align-items`

Controla cómo se alinean los elementos a lo largo del eje transversal.

- `flex-start`: Los elementos se alinean al **inicio** del eje transversal.
- `flex-end`: Los elementos se alinean al **final** del eje transversal.
- `center`: Los elementos se alinean en el **centro** del eje transversal.
- `baseline`: Los elementos se alinean **según su línea base** de texto.
- `stretch`: Los elementos **se estiran para llenar** el contenedor.

```css
.contenedor {
    display: flex;
    align-items: center;
}
```

### 3.3. `flex-direction`

Define la dirección del eje principal.

- `row`: Los elementos se organizan en una **fila horizontal** ***(valor predeterminado)***.
- `row-reverse`: Los elementos se organizan en una **fila horizontal en orden inverso**.
- `column`: Los elementos se organizan en una **columna vertical**.
- `column-reverse`: Los elementos se organizan en una **columna vertical en orden inverso**.

```css
.contenedor {
    display: flex;
    flex-direction: column;
}
```

### 3.4. `flex-wrap`

Determina si los elementos deben ajustarse o no cuando el contenedor es más pequeño que la suma de los elementos.

- `nowrap`: Los elementos **no se ajustan** ***(valor predeterminado)***.
- `wrap`: Los elementos **se ajustan a la siguiente línea si es necesario**.
- `wrap-reverse`: Los elementos **se ajustan a la siguiente línea en orden inverso**.

```css
.contenedor {
    display: flex;
    flex-wrap: wrap;
}
```

### 3.5. `align-content`

Controla el espaciado entre las líneas de elementos en un contenedor cuando hay espacio adicional en el eje transversal.

- `flex-start`: Las líneas **se alinean al inicio** del eje transversal.
- `flex-end`: Las líneas **se alinean al final** del eje transversal.
- `center`: Las líneas **se alinean en el centro** del eje transversal.
- `space-between`: Las líneas **se distribuyen uniformemente** con el primer y último línea alineadas a los bordes.
- `space-around`: Las líneas **se distribuyen uniformemente con espacio igual** alrededor de cada línea.
- `stretch`: Las líneas **se estiran para llenar** el espacio disponible.

```css
.contenedor {
    display: flex;
    align-content: space-between;
    flex-wrap: wrap;
}
```

## 4. Ejemplos Prácticos

### Ejemplo 1: Distribución de Elementos en el Eje Principal

```html
<div class="contenedor">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
</div>
```

```css
.contenedor {
    display: flex;
    justify-content: space-between;
}
.item {
    background-color: #f2f2f2;
    padding: 10px;
    margin: 5px;
}
```

### Ejemplo 2: Flexbox en Columnas

```html
<div class="contenedor">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
</div>
```

```css
.contenedor {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.item {
    background-color: #f2f2f2;
    padding: 10px;
    margin: 5px;
}
```

### Ejemplo 3: Ajuste de Elementos con Flex Wrap

```html
<div class="contenedor">
    <div class="item">Item 1</div>
    <div class="item">Item 2</div>
    <div class="item">Item 3</div>
    <div class="item">Item 4</div>
    <div class="item">Item 5</div>
    <div class="item">Item 6</div>
</div>
```

```css
.contenedor {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}
.item {
    background-color: #f2f2f2;
    padding: 20px;
    margin: 10px;
    flex: 1 1 100px;
}
```

## 5. Ejercicios Prácticos

1. **Distribución Horizontal y Vertical**: Crea un contenedor con varios elementos y usa `justify-content` y `align-items` para alinear los elementos en el centro tanto horizontal como verticalmente.
2. **Galería de Imágenes**: Crea una galería de imágenes que se ajusten en filas con `flex-wrap` y asegúrate de que todas las imágenes tengan el mismo tamaño.
3. **Layout de Página Completo**: Usa Flexbox para crear un layout de página completo con un encabezado, barra de navegación, contenido principal con dos columnas (contenido y barra lateral), y un pie de página.

## 6. Recursos Adicionales

- [CSS Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [MDN Web Docs - Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
