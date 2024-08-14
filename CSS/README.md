# CSS (Cascading Style Sheets / Hojas de Estilo en Cascada) 
Es un lenguaje de diseño/estilado declarativo para describir la presentación de un documento, en nuestro caso HTML.

Con este mismo tenemos el segundo pilar de la web:
1) **HTML** -> Lenguaje de marcado -> *Marcado*
2) **CSS** -> Lenguaje de diseño -> *Estilado*
3) **JavaScript** -> Lenguaje de programación -> *Interacción*

El lanzamiento inicial de CSS fue el 17 de diciembre de **1996** y el primer navegador en darle soporte fue Internet Explorer 3.

El lenguaje tiene una especificación que es mantenida por el *World Wide Web Consortium (W3C)*. Eso hace que sea predecible y que en todos los navegadores se vea de la misma manera los diseños que realizamos.

Con respecto a su nombre, las **Hojas de Estilos** son una _colección de reglas_ que escribimos en el lenguaje y que aplicamos en un documento para darle un diseño. Que sea en **Cascada** se refiere a la forma en la que se aplican las reglas/diseños al documento, siguiendo un _orden_, una _especificidad_, una _importancia_, los _autores_, etc. Esto hace que se __sobrescriban__ las reglas dependiendo del sitio en el que estén, formando así una cascada.
    
## Documentación:
* [MDN](https://developer.mozilla.org/es/docs/Web/CSS)   
* [Google Chrome](https://web.dev/learn/css?hl=es)           

## Estilos del navegador:
__Estilos por defecto__ para cualquier documento HTML que _varían en base al navegador_ (Chrome, Firefox, Safari, etc). Lo que nosotros vamos a hacer es __sobreescribirlos__. _(Se pueden ver inspeccionando los elementos desde el navegador)_


## Semántica de CSS:
```css
    selector {
        propiedad: valor;  /* <- Declaración */
    }
```

___

## Estilos en HTML:
*  __Etiqueta \<style>:__
    
    Una etiqueta que suele colocarse dentro de __\<head>__, aunque pueda colocarse en cualquier otro sitio.

    ejemplo:
    ```html
    <style>
        selector {
            propiedad: valor;     
        }
    </style>
    ```
* __En Línea:__

    Estilos declarados como __atributos__ en los elementos HTML. __No son recomendados__.

    ejemplo:
    ```html
    <h1 style="{color: blue}">
        Hola Mundo
    </h1>
    ```
* __Vinculación:__

    Estilos __separados__ en un archivo con __extensión _.css___

    Son los más recomendados para una mejor __organización__, __prolijidad__ y __reutilización__

    ejemplo:
    
    __HTML__
    
    ```html
    <link rel="stylesheets" href="nombre.css">
    ```
    _(Dentro de __\<head>__)_
    
    El documento va a utilizar las declaraciones que encuentre en el archivo "nombre.css"
___
## Selectores:
* __Etiquetas:__

    Selecciona __todas__ las ocurrencias con esa etiqueta y les aplica las declaraciones.
    
    ejemplo:
    ```css
    h1 {
        color: blue;
    }     
    ```   
    
* __Clases:__

    Selecciona __todas__ las ocurrencias con esa clase y les aplica las declaraciones. 
    
    ejemplo: 
    
    ```html
    <etiqueta class="nombreDeClase">
    ```
    ```css
    /* Punto para las clases */
    .nombreDeClase {
        propiedad: valor;
    }
    ```
* __ID:__
 
    Selecciona el elemento con esa __identificación__ y les aplica las declaraciones. 
    
    ejemplo: 
    
    ```html
    <etiqueta id="identificacion">
    ```
    ```css
    /* Hash para las IDs */
    #identificacion {
        propiedad: valor;
    }
    ```
    Siempre vamos a querer __reutilizar__ nuestros estilos, por ende no es recomendado __abusar__ de las __identificaciones__.


    ## Especificidad:

    1) __Estilos en línea__ -> 
        ```html
        <h1 style="{color: blue}">Hola Mundo</h1>
        ```
    2) __Identificadores__ ->

        __HTML:__ 
        ```html
        <h1 id="identificador">Hola Mundo</h1>
        ```
        __CSS:__ 
        ```css
        #identificador {
            color: blue;
        }
        ```
    3) __Clases__ ->

        __HTML:__ 
        ```html
        <h1 class="nombreDeClase">Hola Mundo</h1>
        ```
        __CSS:__ 
        ```css
        .nombreDeClase {
            color: blue;
        }
        ```
    
    4) Etiquetas ->

        __HTML:__
        ```html
        <h1>Hola Mundo</h1>
        ```
        __CSS:__ 
        ```css
        h1 {
            color: blue;
        }
        ```

___

## Tipos de colores:
```css
/* Valores de palabras clave */
color: currentcolor; 
/* Se utiliza a veces de forma
automática para bordes */
/* Toma el valor actual del elemento
superior o del texto (en bordes) */

/* Valores <named-color> */
color: red;
color: orange;
color: tan;
color: rebeccapurple;
/* Palabras reservadas para la mayoría
de colores (se pueden ver diferente
en cada navegador)*/


/* Valores <hex-color> */
color: #090; 
/* Son equivalentes */
color: #009900;

color: #090a;
/* Para manejar la opacidad*/
color: #009900aa;

/* Valores <rgb()> */
color: rgb(34, 12, 64, 0.6);
color: rgba(34, 12, 64, 0.6);
color: rgba(34 12 64 / 0.3);
color: rgba(34.6 12 64 / 30%);
/* Ya no se usan */

color: rgb(34 12 64 / 0.6);
color: rgb(34 12 64 / 60%);
/* Formas modernas */

/* Valores <hsl()> */
color: hsl(30, 100%, 50%, 0.6);
color: hsla(30, 100%, 50%, 0.6);
color: hsl(30 100% 50% / 0.6);
color: hsla(30 100% 50% / 0.6);
color: hsl(30 100% 50% / 60%);
color: hsla(30.2 100% 50% / 60%);

/* Valores Globales */
color: inherit;
color: initial;
color: unset;
```
[MDN CSS -> Color](https://developer.mozilla.org/es/docs/Web/CSS/color)

___



## [Herencia en CSS](https://developer.mozilla.org/es/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)



___

## [Selectores Combinados](https://developer.mozilla.org/es/docs/Learn/CSS/Building_blocks/Selectors/Combinators)


___ 

## [Modelo de la Caja (Box-Model)](https://developer.mozilla.org/es/docs/Learn/CSS/Building_blocks/The_box_model)



