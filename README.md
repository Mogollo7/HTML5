# HTML

**HTML** es fundamental en casi todos los aspectos relacionados con la programación, especialmente si deseas trabajar profesionalmente como programador.

# Tabla de Contenidos

1. [HTML](#html)
2. [¿Qué es HTML?](#qué-es-html)
3. [Estructura de una Etiqueta HTML](#estructura-de-una-etiqueta-html)
4. [División en Bloques](#división-en-bloques)
5. [Estructura del Documento HTML](#estructura-del-documento-html)
6. [Creación de un Documento HTML](#creación-de-un-documento-html)
7. [Etiquetas](#etiquetas)
   - [`<!DOCTYPE html>`](#doctype-html)
   - [`<html>`](#html)
   - [`<head>`](#head)
   - [`<body>`](#body)
   - [`<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`](#h1-h2-h3-h4-h5-h6)
   - [`<p>`](#p)
   - [`<a>`](#a)
   - [`<img>`](#img)
   - [`<ul>` y `<ol>`](#ul-y-ol)
   - [`<div>`](#div)
   - [`<span>`](#span)
   - [`<br>`](#br)
   - [`<hr>`](#hr)
   - [`<form>`](#form)
   - [`<button>`](#button)
   - [`<header>` y `<footer>`](#header-y-footer)
   - [`<section>`](#section)
8. [Atributos Comunes en HTML](#atributos-comunes-en-html)
   - [`id`](#id)
   - [`class`](#class)
   - [`href`](#href)
   - [`src`](#src)
   - [`alt`](#alt)
   - [`action` y `method`](#action-y-method-en-formularios)


## ¿Qué es HTML?

**HTML (HyperText Markup Language)** es el lenguaje estándar para crear páginas web en la actualidad. Todos los demás lenguajes utilizados para páginas web deben ser compilados o interpretados en **HTML**. Este lenguaje describe la estructura de la página web, especificando qué elementos se mostrarán y cómo se presentarán. Se compone de etiquetas que indican párrafos, enlaces, títulos, entre otros.

La organización básica de un documento **HTML** sigue una estructura jerárquica en forma de árbol, en la cual cada elemento puede contener otros elementos dentro de sí. Esta forma de anidación permite la creación de bloques de contenido bien definidos, facilitando tanto la legibilidad como la accesibilidad.

## Estructura de una Etiqueta HTML

Una etiqueta **HTML** consta de tres partes: 
1. **Apertura**: Contiene el nombre de la etiqueta.
2. **Contenido**: Es lo que va dentro de la etiqueta.
3. **Cierre**: Incluye el nombre de la etiqueta precedido de una barra `/`.

### División en Bloques

Al programar en **HTML**, notarás que el contenido se organiza en bloques. Cada bloque puede contener otros bloques, lo que permite una estructura jerárquica clara y ordenada. Por ejemplo, un encabezado principal puede contener subtítulos, párrafos o listas, dividiendo así el contenido en secciones manejables y bien definidas.

Esta estructura en bloques facilita la comprensión y el mantenimiento del código, permitiendo a los desarrolladores trabajar de manera más eficiente y organizada. A continuación, se muestra un ejemplo de esto.

### Estructura del Documento HTML

En un documento **HTML**, comenzamos con la etiqueta `<html>`, que es la raíz de nuestra página. Dentro de esta etiqueta, encontramos la etiqueta `<head>`, que se utiliza para añadir instrucciones y metadatos, así como otros tipos de código que pueden ser necesarios para la página web, como enlaces a hojas de estilo o scripts.

A continuación, tenemos la etiqueta `<body>`, donde se incluye todo el contenido visible de la página web. Este es el lugar donde se presentarán elementos como texto, imágenes, enlaces y más.

```html
<!DOCTYPE html>
<html>
   <head>
       <title>Título Principal</title>
   </head>
   <body>
       <h1>Título Principal de la Página</h1>
       <p>Este es un párrafo que contiene el texto visible para los usuarios.</p>
   </body>
</html>
```

Es importante considerar que, en el apartado de `<head>`, el `<title>` será fundamental para que tu página web sea encontrada en cualquier buscador. Este título sirve como base para que el motor de búsqueda muestre las opciones coincidentes.

## Creación de un Documento HTML

Para empezar a programar, debemos crear un documento llamado `index.html`. La extensión `.html` indica al editor de texto que es un archivo **HTML**, y `index` es un estándar que se utiliza para nombrar el archivo principal.

Para iniciar, abre `index.html`, copia un signo de exclamación (`!`) y luego presiona `Tab`. Esto utilizará **Emmet**, una herramienta de **Visual Studio Code** que permite escribir código de manera más rápida y eficiente, similar al `System.out.println` (sout) en Java.

### Etiquetas

#### `<!DOCTYPE html>`

La primera etiqueta, llamada `<!DOCTYPE html>`, indica que estamos utilizando **HTML5**. Si eliminamos esta etiqueta, el navegador considerará que estamos programando con un código antiguo, lo que podría generar errores.

```html
<!DOCTYPE html>
<html>
   <head>
       <title>Título de la Página</title>
   </head>
   <body>
       <h1>Título Principal</h1>
       <p>Este es un párrafo que contiene el texto visible para los usuarios.</p>
   </body>
</html>
```

### `<html>`

La etiqueta `<html>` es la raíz de cualquier documento **HTML**. Cada documento debe incluir esta etiqueta para funcionar correctamente.

```html
<html>
    <!-- Contenido del documento HTML como head, body, etc. -->
</html>
```

### `<head>`

Dentro de la etiqueta `<head>`, podemos agregar características que afectarán nuestra página web, aunque no sean visibles para el usuario. Por ejemplo, la etiqueta `<title>` define el título de nuestra página web, que podremos ver al abrir el archivo en el navegador.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Página</title>
</head>
</html>
```

### `<body>`

La etiqueta `<body>` es donde se incluirá todo el contenido visible de nuestra web.

#### `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`

Las etiquetas de encabezado `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>` y `<h6>` se utilizan dentro del `<body>` para definir títulos y subtítulos en el contenido de nuestra página web. El número que sigue a la letra "h" indica el nivel de encabezado y determina el tamaño del texto.

```html
<!DOCTYPE html>
<html>
<head>
</head>
<body>
    <h1>Título Principal de la Página</h1>
    <h2>Subtítulo de la Sección</h2>
    <h3>Subsección Importante</h3>
    <h4>Título Menor</h4>
    <h5>Título de Tercera Clase</h5>
    <h6>Título de Cuarta Clase</h6>
</body>
</html>
```
---
<!DOCTYPE html>
<html>
<head>

</head>
<body>
    <h1>Título Principal de la Página</h1>
    <h2>Subtítulo de la Sección</h2>
    <h3>Subsección Importante</h3>
    <h4>Título Menor</h4>
    <h5>Título de Tercera Clase</h5>
    <h6>Título de Cuarta Clase</h6>
</body>
</html>


### `<p>`

La etiqueta `<p>` se utiliza para definir párrafos de texto dentro del contenido visible de la página. Permite organizar el texto en bloques, facilitando su lectura y presentación.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Párrafo</title>
</head>
<body>
    <h1>Título Principal de la Página</h1>
    <p>Este es un párrafo que proporciona información sobre el contenido de la página.</p>
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>

</head>
<body>
    <h1></h1>
    <p>Este es un párrafo que proporciona información sobre el contenido de la página.</p>
</body>
</html>

### `<a>`

La etiqueta `<a>` se utiliza para crear hipervínculos que conectan a otras páginas o recursos en la web. Debes proporcionar el atributo `href` que contiene la URL a la que se enlazará.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Enlace</title>
</head>
<body>
    <h1>Título Principal</h1>
    <p>Visita <a href="https://www.ejemplo.com">nuestro sitio web</a> para más información.</p>
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>

</head>
<body>
    <h1></h1>
    <p>Visita <a href="https://github.com/Mogollo7?tab=repositories">nuestro sitio web</a> para más información.</p>
</body>
</html>

### `<img>`

La etiqueta `<img>` se utiliza para insertar imágenes en la página. Debe incluir el atributo `src` que especifica la ruta de la imagen, y el atributo `alt` para proporcionar una descripción alternativa.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Imagen</title>
</head>
<body>
    <h1>Título Principal</h1>
    <img src="ruta o carpeta/imagen.jpg" alt="Descripción de la imagen" width="tamaño">
</body>
</html>
```
<figure style="text-align: center;">
<<<<<<< Updated upstream
  <img src="HTML5.png" alt="" width="400" height="" />
=======
  <img src="HTML5.png" alt="" width="400"/>
>>>>>>> Stashed changes
  <figcaption><strong>Calculadora</strong></figcaption>
</figure>

### `<ul>` y `<ol>`

Las etiquetas `<ul>` (lista desordenada) y `<ol>` (lista ordenada) se utilizan para crear listas en el contenido. Cada elemento de la lista se define con la etiqueta `<li>`.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Listas</title>
</head>
<body>
    <h1>Título Principal</h1>
    <h2>Lista Desordenada</h2>
    <ul>
        <li>Elemento uno</li>
        <li>Elemento dos</li>
        <li>Elemento tres</li>
    </ul>
    <h2>Lista Ordenada</h2>
    <ol>
        <li>Elemento uno</li>
        <li>Elemento dos</li>
        <li>Elemento tres</li>
    </ol>
</body>
</html>
```

<!DOCTYPE html>
<html>
<body>
    <h4>Título Principal</h1>
    <h5>Lista Desordenada</h2>
    <ul>
        <li>Elemento uno</li>
        <li>Elemento dos</li>
        <li>Elemento tres</li>
    </ul>
    <h5>Lista Ordenada</h2>
    <ol>
        <li>Elemento uno</li>
        <li>Elemento dos</li>
        <li>Elemento tres</li>
    </ol>
</body>
</html>

### `<div>`

La etiqueta `<div>` se utiliza para agrupar contenido y crear secciones. No tiene un significado semántico por sí misma, pero es útil para aplicar estilos o scripts a un bloque de contenido ademas de que era muy utilizado antes de la llegada de las etiquetas semánticas de HTML5, como `<header>`, `<footer>`, `<article>`, y `<section>`.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de División</title>
</head>
<body>
    <div>
        <h1>Título Principal</h1>
        <p>Este es un párrafo dentro de un bloque de división.</p>
    </div>
</body>
</html>
```

### `<span>`

La etiqueta `<span>` es similar a `<div>`, pero se utiliza para aplicar estilos a partes específicas de texto dentro de un párrafo sin crear un bloque nuevo.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Span</title>
</head>
<body>
    <h1>Título Principal</h1>
    <p

>Este es un <span style="color:red;">texto destacado</span> dentro de un párrafo.</p>
</body>
</html>
```

### `<br>`

La etiqueta `<br>` se utiliza para forzar un salto de línea. Es útil cuando deseas separar líneas dentro de un párrafo sin crear un nuevo bloque.


```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Salto de Línea</title>
</head>
<body>
    <h1>Título Principal</h1>
    <p>Este es un párrafo.<br>Este texto aparece en la siguiente línea.</p>
</body>
</html>
```
<!DOCTYPE html>
<html>

<body>
    <h1></h1>
    <p>Este es un párrafo.<br>Este texto aparece en la siguiente línea.</p>
</body>
</html>

### `<hr>`

La etiqueta `<hr>` se utiliza para insertar una línea horizontal, que puede servir como separador visual entre secciones de contenido.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Línea Horizontal</title>
</head>
<body>
    <h1>Título Principal</h1>
    <p>Este es un párrafo antes de la línea horizontal.</p>
    <hr>
    <p>Este es un párrafo después de la línea horizontal.</p>
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>
 
</head>
<body>
    <h1></h1>
    <p>Este es un párrafo antes de la línea horizontal.</p>
    <hr>
    <p>Este es un párrafo después de la línea horizontal.</p>
</body>
</html>

### `<form>`

La etiqueta `<form>` se utiliza para crear formularios que permiten a los usuarios enviar datos. Dentro de un formulario, puedes incluir diversas entradas como campos de texto, botones, etc.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Formulario</title>
</head>
<body>
    <h1>Título Principal</h1>
    <form action="ruta/al/servidor" method="post">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" placeholder="Escribe tu nombre">
        <input type="submit" value="Enviar">
    </form>
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>

</head>
<body>
    <h1></h1>
    <form action="servidor" method="post">
        <label for="nombre">Nombre:</label>
        <input type="text" id="nombre" name="nombre" placeholder="Escribe tu nombre">
        <input type="submit" value="Enviar">
    </form>
</body>
</html>

### `<button>`

La etiqueta `<button>` se utiliza para crear botones interactivos. Puedes incluir texto y otros elementos HTML dentro de ella.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Botón</title>
</head>
<body>
    <h1>Título Principal</h1>
    <button type="button" onclick="alert('¡Hola!')">Haz clic aquí</button>
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>

</head>
<body>
    <h1></h1>
    <button type="button" onclick="alert('¡Hola!')">Haz clic aquí</button>
</body>
</html>

### `<header>` y `<footer>`

Las etiquetas `<header>` y `<footer>` se utilizan para definir la cabecera y el pie de una página o sección. Generalmente incluyen información como el título de la página, el autor, la fecha, o enlaces de navegación.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Header y Footer</title>
</head>
<body>
    <header>
        <h1>Título del Blog</h1>
    </header>
    <footer>
        <p>Derechos reservados © 2024</p>
    </footer>
</body>
</html>
```
<!DOCTYPE html>
<html>
<head>
    
</head>
<body>
    <header>
        <h4>titulo</h4>
    </header>
    <footer>
        <p>Derechos reservados © 2024</p>
    </footer>
</body>
</html>

### `<section>`

La etiqueta `<section>` se utiliza para agrupar contenido relacionado. Cada sección puede tener su propio encabezado y se considera un bloque de contenido independiente.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Ejemplo de Sección</title>
</head>
<body>
    <h1>Título Principal</h1>
    <section>
        <h2>Título de la Sección</h2>
        <p>Este es el contenido de la sección.</p>
    </section>
</body>
</html>
```

### Atributos Comunes en HTML

#### `id`

- **Descripción**: El atributo `id` se utiliza para identificar de manera única un elemento dentro del documento HTML. Cada `id` debe ser único en una página.
- **Ejemplo**:
    ```html
    <h1 id="titulo-principal">Título Principal</h1>
    ```

#### `class`

- **Descripción**: El atributo `class` se utiliza para agrupar varios elementos bajo una misma clase, permitiendo aplicar estilos a todos ellos simultáneamente mediante CSS.
- **Ejemplo**:
    ```html
    <p class="texto-importante">Este es un párrafo importante.</p>
    ```

#### `href`

- **Descripción**: Este atributo se usa en la etiqueta `<a>` para especificar la URL a la que se vincula el enlace.
- **Ejemplo**:
    ```html
    <a href="https://github.com/Mogollo7?tab=repositories">Visita nuestro sitio web</a>
    ```

#### `src`

- **Descripción**: Utilizado en la etiqueta `<img>`, especifica la ubicación de la imagen que se desea mostrar.
- **Ejemplo**:
    ```html
    <img src="ruta a la imagen.jpg" alt="Descripción de la imagen">
    ```

#### `alt`

- **Descripción**: Proporciona una descripción alternativa para una imagen, que se muestra si la imagen no se puede cargar o para ayudar a las personas con discapacidades visuales.
- **Ejemplo**:
    ```html
    <img src="ruta a la imagen.jpg" alt="Descripción de la imagen">
    ```

#### `action` y `method` (en formularios)

- **action**: Especifica la URL a la que se enviarán los datos del formulario cuando se envíe.
- **method**: Indica el método HTTP que se utilizará para enviar los datos (generalmente `GET` o `POST`).

Los métodos `GET` y `POST` son dos formas de enviar datos en formularios web, cada uno con sus propias características. Mientras que `GET` envía los datos a través de la URL, lo que los hace visibles y potencialmente inseguros, `POST` los envía en el cuerpo de la solicitud, proporcionando mayor privacidad. Además, `GET` tiene limitaciones de longitud en la URL, lo que lo hace inapropiado para grandes volúmenes de datos, mientras que `POST` no presenta estas restricciones.

- **Ejemplo**:
    ```html
    <form action="ruta al servidor" method="post">
<<<<<<< Updated upstream
    ```
=======
    ```
>>>>>>> Stashed changes
