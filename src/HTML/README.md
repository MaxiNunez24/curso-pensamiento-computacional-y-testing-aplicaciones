[**Volver al inicio**](../../)

# HTML (HyperText Markup Language / *Lenguaje de Marcado de HyperTexto*)

## 1. ¿Qué es HTML?

Es el **lenguaje estándar** utilizado para crear páginas web. HTML define la **estructura básica** de un sitio web utilizando **elementos** y **etiquetas** que permiten organizar y mostrar **contenido** como *texto*, *imágenes*, *videos*, *enlaces*, *formularios*, y más.
**No es un lenguaje de programación**, *como si lo es **[JavaScript](../JS)***, **Ni de estilado**, *como si lo es **[CSS](../CSS/)***,  por lo que sólo vamos a "marcar", describir o estructurar nuestra página con él.

## 2. Un Poco de Historia 

HTML fue creado por **Tim Berners-Lee** en **1991** mientras trabajaba en el CERN (Organización Europea para la Investigación Nuclear). Desde entonces, HTML ha **evolucionado** significativamente, con la última versión importante, **HTML5**, lanzada en **2014**. HTML5 introdujo nuevas *etiquetas* y *capacidades*, como **soporte para *multimedia***, *gráficos* y *aplicaciones interactivas* sin la necesidad de plugins adicionales.

## 3. La Sintaxis Básica de HTML

HTML utiliza una serie de **etiquetas** que están delimitadas por `<` y `>`. Estas etiquetas suelen aparecer en **pares**, con una **etiqueta de apertura** y una **etiqueta de cierre**, que *envuelven* el **contenido** al que se aplican. Es decir, los **Elementos HTML** son el **contenido de la página** intercalado entre las etiquetas. Por ejemplo, el **elemento** `<p>` incluiría tanto la *etiqueta de apertura* `<p>` como el *contenido del párrafo*, así como la *etiqueta de cierre* `</p>`. La mayoría de los elementos siguen esta estructura:

```html
<etiqueta>Contenido</etiqueta>
```

![Estructura Elementos HTML](../images/estructura-elemento-HTML.jpg)

Por ejemplo, un párrafo en HTML se escribiría así:

```html
<p>Este es un párrafo en HTML.</p>
```

## 4. Estructura de un Documento HTML

Un documento HTML básico tiene una estructura estándar que incluye las siguientes secciones:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Primera Página Web</title>
</head>
<body>
    <h1>¡Hola, mundo!</h1>
    <p>Este es un párrafo en mi primera página web.</p>
</body>
</html>
```

### Descripción de las Etiquetas Principales

- `<!DOCTYPE html>`: Declara que el **documento está en HTML5**.
- `<html>`: Es la **raíz** del documento HTML.
- `<head>`: Contiene **metadatos** como el *título* de la página, *enlaces* a hojas de estilo, y otros elementos que **no se muestran** directamente en la página.
- `<title>`: Define el **título** de la página que aparece en la pestaña del navegador.
- `<meta charset="UTF-8">`: Especifica la **codificación de caracteres**, permitiendo el uso de *caracteres especiales*.
- `<body>`: Contiene todo el contenido que **se mostrará** en la página web.

## 5. Semántica en HTML

La semántica en HTML se refiere al uso de etiquetas que **describen adecuadamente** el tipo de contenido que contienen. Esto mejora la **accesibilidad**, el **SEO***(Search Engine Optimization/Optimización para motores de búsqueda)*, y la **comprensión del código** tanto por *humanos* como por *motores de búsqueda*.

**Ejemplos de etiquetas semánticas**:

- `<header>`: **Encabezado** de una *sección* o *página*.
- `<nav>`: Contiene **enlaces de navegación**.
- `<main>`: **Contenido principal** de la página.
- `<article>`: Un **artículo independiente**.
- `<footer>`: **Pie de página**.

## 6. Conceptos Básicos de HTML

### 6.1. Listas

Existen *dos tipos principales* de **listas** en HTML:

- **Listas ordenadas** (`<ol>`):

```html
<ol>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
</ol>
```

- **Listas desordenadas** (`<ul>`):

```html
<ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
</ul>
```

### 6.2. Enlaces

Los enlaces se crean con la etiqueta `<a>` *(Pueden contener tanto referencias internas como externas)*:

```html
<a href="https://www.example.com">Visita Example Externa</a>

<a href="../assets/examples/index.html">Visita Example Interna</a>
```

### 6.3. Imágenes

Las imágenes se *insertan* utilizando la etiqueta `<img>` *(Al ser un elemento reemplazable no hace falta cerrar la etiqueta)*:

```html
<img src="assets/imagen.jpg" alt="Descripción de la imagen">
```

### 6.4. Tablas

Las tablas se estructuran con etiquetas como `<table>`, `<tr>` *(fila)*, `<td>` *(celda)*, y `<th>` *(encabezado de columna)*:

```html
<table>
    <tr>
        <th>Encabezado 1</th>
        <th>Encabezado 2</th>
    </tr>
    <tr>
        <td>Dato 1</td>
        <td>Dato 2</td>
    </tr>
</table>
```

## 7. Recursos Adicionales

- [MDN Web Docs - HTML](https://developer.mozilla.org/es/docs/Web/HTML)
- [W3Schools - Tutorial de HTML](https://www.w3schools.com/html/)

## 8. Ejercicios Prácticos

1. **Crear una página HTML básica**: Creen una página con un *título*, un *par de párrafos*, una *imagen* y un *enlace*.
2. **Experimentar con etiquetas semánticas**: Modificar la *estructura de la página* para incluir **etiquetas semánticas** como `<header>`, `<nav>`, `<main>`, `<article>`, y `<footer>`.

## 9. Preguntas Frecuentes

1. **¿Es obligatorio cerrar todas las etiquetas en HTML?**
   - Sí, la mayoría de las etiquetas **deben cerrarse** para que el código sea válido, aunque hay algunas **excepciones** como `<img>` y `<br>`.

2. **¿Qué es HTML5 y por qué es importante?**
   - **HTML5** es la versión *más reciente* de HTML y es importante porque *introduce nuevas etiquetas*, **mejora** *la semántica* y *accesibilidad*, y **permite el uso de multimedia** sin necesidad de plugins.