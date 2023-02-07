# ¿Cómo empezar con HTML?

[Página de referencia](https://en.wikipedia.org/wiki/HTML_element)

# Etiquetas

## Etiquetas estructurales

* `<html>`: La raíz del elemento HTML. Contiene todos los elementos.
* `<head>`: Contiene metadatos sobre el documento, como el título, el autor, los distitnos tipos de enlaces con otros ficheros, etc.
* `<body>`: Tiene el contenido del documento, como texto, imágenes, enlaces, etc.

### Etiquetas básicas del Head

* `<title>`: Contiene el título del documento.
* `<link>`: Enlaza con un fichero externo, como un CSS o un JS.
* `<meta>`: Contiene metadatos sobre el documento, como el autor, la descripción, etc.
* `<style>`: Contiene estilos CSS.
* `<script>`: Contiene código JavaScript.

### Generar un fichero HTML básico con título.

Crear un fichero HTML con el nombre `index.html`.

Para obetener el código base de HTML usando VSCode, escribir `html:5` y pulsar `Enter`.

Para ejecutar el fichero HTML, pulsar `Ctrl + Shift + P` y escribir `Live Server: Open with Live Server`.

A continuación, clicaremos sobre el fichero `index.html` y le daremos a `Open with Live Server`.

```apache
<!-- Comentario en HTML -->
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, 
        initial-scale=1.0">
    <title>Document</title>
</head>
<body>
</body>
</html>
```

## Etiquetas básicas del Body

Dentro de todas las etiquetas que pueden existir, las más útiles son las siguientes:
![E](./assets/estructura_html.jpg)

### Estructuras básicas

* `<header>`: Contiene el encabezado del documento.
* `<nav>`: Contiene enlaces de navegación.
* `<main>`: Contiene el contenido principal del documento.
* `<section>`: Contiene el apartado principal del documento.
* `<article>`: Contiene los distintos datos del documento.
* `<aside>`: Contiene información adicional del documento.
* `<footer>`: Contiene el pie de página del documento.

### Componentes básicos

* Encabezados, van del 1 al 6, siendo el 1 el más grande y el 6 el más pequeño.
  * `<h1>`: Encabezado 1
  * `<h2>`: Encabezado 2
  * `<h3>`: Encabezado 3
  * `<h4>`: Encabezado 4
  * `<h5>`: Encabezado 5
  * `<h6>`: Encabezado 6
* `<p>`: Párrafo
* `<br>`: Salto de línea
* `<hr>`: Línea horizontal
* `<a>`: Enlace
* `<img>`: Imagen
* `<form>`: Formulario [Apartado de formularios](#formularios)
  * `<input>`: Herramienta básica para la obtención de datos.
  * `<label>`: Etiqueta que asigna un elemento de entrada a un texto.
  * `<textarea>`: Área de texto, hecha para insertar textos o párrafos largos.
  * `<select>`: Contiene distintas opciones (`<option>`)

### Listas

* `<ul>`: Lista no ordenada.
* `<ol>`: Lista ordenada.

Dentro de cada lista se coloca `<li>` para cada elemento de la lista.

### Tablas

Estructura básica de la tabla:

* `<table>`: Base para crear una tabla.
* `<thead>`: Cabecera de la tabla.
* `<tbody>`: Cuerpo de la tabla.
* `<tfoot>`: Pie de la tabla.

Elementos que puede contener una tabla:

* `<tr>`: Fila.
* `<th>`: Celda en negrita.
* `<td>`: Celda.
* `<caption>`: Título.

# Formularios

[Página de referencia](https://www.uv.es/~sto/libros/cyberdisk/alice/html/s1_6.htm)

Acceder a [prueba de formularios](./examples/forms.html) para ver mejor el funcionamiento de los formularios.

# HTML Semántico 

Es importante a la hora de crear nuestras interfaces utilizar los elementos de HTML de contenido del texto para organizar bloques o secciones de contenido colocados entre los tags de apertura y cierre. Es importante para la accessibility y el SEO, que estos elementos se identifiquen con el objetivo o la estructura de ese contenido. De esta forma las páginas podrán estar mejor indexadas y aparecer mejor posicionadas ante las búsquedas de nuestros usuarios. 

Una pista para saber que no estamos usando la semántica del HTML correctamente es ver nuestro código plagado de `<div>` y `<p>` anidados, también podemos hacer uso de un [validador](https://validator.w3.org/) online que validan nuestra estructura y semántica HTML. 

Estos son algunos de los elementos que debemos utilizar para aprovechar al máximo la semántica de HTML:

- El elemento `<details>` crea un widget de divulgación en el que la información es visible solo cuando el widget se cambia a un estado "open". Se debe proporcionar un resumen o etiqueta utilizando el elemento `<summary>` 
- El elemento `<figure>` representa un contenido normalmente de tipo imagen o esquema, normalmente se utiliza para envolver elementos de tipo `<img>`
- El elemento `<figcaption>` se utiliza dentro de la etiqueta `<figure>` para definir una leyenda o texto descriptivo de la figura
- El elemento `<dt>`se utiliza para envolver un término que será posteriormente descrito dentro de la etiqueta `<dd>`
- El elemento `<address>` indica que el HTML contenido en el da datos de contacto de la persona, organización, o empresa.
- El elemento `<abbr>` permite envolver abreviaciones e incluir una descripción usando el atributo title.

Existen más etiquetas que se deberían usar para aprovechar la correcta semántica de HTML, las podrás encontrar [aquí](https://developer.mozilla.org/en-US/docs/Web/HTML/Element).