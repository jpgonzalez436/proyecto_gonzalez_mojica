# 🌐 Guía Básica de HTML

> **HTML (HyperText Markup Language)** es el lenguaje utilizado para estructurar el contenido de las páginas web.

---

## 📚 Índice

1. [¿Qué es HTML?](#-qué-es-html)
2. [Estructura básica](#-estructura-básica-de-un-documento-html)
3. [Etiquetas y elementos](#-etiquetas-y-elementos)
4. [Atributos](#-atributos)
5. [Texto y títulos](#-texto-y-títulos)
6. [Enlaces](#-enlaces)
7. [Imágenes](#-imágenes)
8. [Listas](#-listas)
9. [Tablas](#-tablas)
10. [Formularios](#-formularios)
11. [Contenedores](#-contenedores)
12. [Etiquetas semánticas](#-etiquetas-semánticas)
13. [Multimedia](#-multimedia)
14. [Comentarios](#-comentarios)
15. [Caracteres especiales](#-caracteres-especiales)
16. [Buenas prácticas](#-buenas-prácticas)
17. [Ejemplo completo](#-ejemplo-completo)

---

# 🧠 ¿Qué es HTML?

HTML es un **lenguaje de marcado**, no un lenguaje de programación.

Se utiliza principalmente para definir la **estructura y el significado del contenido** de una página web.

Una página normalmente combina:

| Tecnología | Función |
|---|---|
| 🟧 **HTML** | Estructura y contenido |
| 🟦 **CSS** | Diseño y apariencia |
| 🟨 **JavaScript** | Interactividad y comportamiento |

### Ejemplo

```html
<h1>Mi página web</h1>
<p>Esta es una página creada con HTML.</p>
```

HTML indica que existe un **título** (`h1`) y un **párrafo** (`p`).

---

# 🏗️ Estructura básica de un documento HTML

Todo documento HTML moderno debería comenzar con una estructura similar a esta:

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Mi página web</title>
</head>

<body>

    <h1>Hola, mundo</h1>
    <p>Mi primera página web.</p>

</body>

</html>
```

## 🔎 Partes principales

### `<!DOCTYPE html>`

Indica al navegador que estamos utilizando **HTML5**.

### `<html>`

Es el elemento raíz que contiene todo el documento.

```html
<html lang="es">
```

El atributo `lang="es"` indica que el contenido está en español.

### `<head>`

Contiene información sobre la página que normalmente no se muestra directamente.

Aquí suelen encontrarse:

- Metadatos
- Título
- Enlaces a CSS
- Scripts
- Configuración de visualización

### `<body>`

Contiene todo el contenido visible de la página.

```html
<body>
    <h1>Título</h1>
    <p>Contenido de la página.</p>
</body>
```

---

# 🧩 Etiquetas y elementos

Una etiqueta normalmente se escribe entre `<` y `>`.

```html
<p>Hola</p>
```

Aquí:

- `<p>` → etiqueta de apertura
- `Hola` → contenido
- `</p>` → etiqueta de cierre

Todo el conjunto constituye un **elemento HTML**.

## Etiquetas de apertura y cierre

```html
<h1>Título</h1>
<p>Párrafo</p>
<strong>Texto importante</strong>
```

## Elementos sin cierre

Algunos elementos no necesitan una etiqueta de cierre:

```html
<img src="foto.jpg" alt="Una fotografía">
<br>
<hr>
<input type="text">
```

---

# ⚙️ Atributos

Los atributos proporcionan información adicional a un elemento.

Se escriben normalmente dentro de la etiqueta de apertura:

```html
<a href="https://www.google.com">Google</a>
```

En este caso:

- `a` → etiqueta
- `href` → atributo
- `"https://www.google.com"` → valor del atributo

### Ejemplo con varios atributos

```html
<img 
    src="imagen.jpg" 
    alt="Paisaje" 
    width="500"
>
```

### Atributos comunes

| Atributo | Uso |
|---|---|
| `id` | Identificador único |
| `class` | Agrupar elementos para CSS/JS |
| `href` | Dirección de un enlace |
| `src` | Ruta de un recurso |
| `alt` | Texto alternativo |
| `title` | Información adicional |
| `style` | Estilos directamente en HTML |
| `name` | Nombre de un elemento de formulario |
| `value` | Valor de un campo |
| `placeholder` | Texto de ayuda en un campo |

---

# ✍️ Texto y títulos

## Títulos

HTML proporciona seis niveles de títulos:

```html
<h1>Título principal</h1>
<h2>Subtítulo</h2>
<h3>Sección</h3>
<h4>Subsección</h4>
<h5>Título pequeño</h5>
<h6>Título muy pequeño</h6>
```

`<h1>` representa el nivel principal y `<h6>` el menor nivel.

### Recomendación

Utiliza los títulos según su **jerarquía**, no solamente por su tamaño visual.

---

## Párrafos

```html
<p>Este es un párrafo.</p>
```

---

## Texto en negrita

```html
<strong>Texto importante</strong>
```

También existe:

```html
<b>Texto en negrita</b>
```

En general, `strong` es preferible cuando el texto tiene **importancia semántica**.

---

## Texto en cursiva

```html
<em>Texto enfatizado</em>
```

También:

```html
<i>Texto en cursiva</i>
```

`em` aporta significado semántico de énfasis.

---

## Saltos de línea

```html
<p>Primera línea<br>Segunda línea</p>
```

---

## Línea horizontal

```html
<hr>
```

Se utiliza para representar una separación temática.

---

# 🔗 Enlaces

Los enlaces se crean mediante `<a>`.

```html
<a href="https://www.google.com">Visitar Google</a>
```

## Abrir en otra pestaña

```html
<a 
    href="https://www.google.com" 
    target="_blank"
    rel="noopener noreferrer"
>
    Google
</a>
```

## Enlace a otra página del proyecto

```html
<a href="contacto.html">Contacto</a>
```

## Enlace dentro de la misma página

Primero se crea un `id`:

```html
<h2 id="contacto">Contacto</h2>
```

Después:

```html
<a href="#contacto">Ir a contacto</a>
```

---

# 🖼️ Imágenes

La etiqueta principal es `<img>`.

```html
<img src="foto.jpg" alt="Descripción de la fotografía">
```

### Atributos importantes

```html
<img 
    src="foto.jpg"
    alt="Paisaje de montaña"
    width="600"
    height="400"
>
```

### `alt`

El atributo `alt` describe la imagen cuando esta no puede visualizarse y mejora la accesibilidad.

---

# 📋 Listas

## Lista desordenada

Utiliza `<ul>` y `<li>`:

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

Resultado conceptual:

- HTML
- CSS
- JavaScript

---

## Lista ordenada

Utiliza `<ol>`:

```html
<ol>
    <li>Encender el computador</li>
    <li>Abrir el navegador</li>
    <li>Crear el proyecto</li>
</ol>
```

Resultado conceptual:

1. Encender el computador
2. Abrir el navegador
3. Crear el proyecto

---

## Listas anidadas

```html
<ul>
    <li>
        Frontend
        <ul>
            <li>HTML</li>
            <li>CSS</li>
            <li>JavaScript</li>
        </ul>
    </li>

    <li>Backend</li>
</ul>
```

---

# 📊 Tablas

Una tabla utiliza principalmente:

- `<table>` → tabla
- `<tr>` → fila
- `<th>` → encabezado
- `<td>` → celda

```html
<table>
    <tr>
        <th>Nombre</th>
        <th>Edad</th>
    </tr>

    <tr>
        <td>Juan</td>
        <td>23</td>
    </tr>
</table>
```

## Estructura más completa

```html
<table>
    <thead>
        <tr>
            <th>Producto</th>
            <th>Precio</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>Teclado</td>
            <td>$50</td>
        </tr>
    </tbody>

    <tfoot>
        <tr>
            <td>Total</td>
            <td>$50</td>
        </tr>
    </tfoot>
</table>
```

---

# 📝 Formularios

Los formularios permiten recibir información del usuario.

```html
<form>

    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre">

    <button type="submit">Enviar</button>

</form>
```

## Tipos comunes de `input`

```html
<input type="text">
<input type="password">
<input type="email">
<input type="number">
<input type="date">
<input type="checkbox">
<input type="radio">
<input type="file">
<input type="submit">
```

## Placeholder

```html
<input 
    type="text"
    placeholder="Escribe tu nombre"
>
```

## Campo obligatorio

```html
<input 
    type="email"
    required
>
```

## Área de texto

```html
<textarea 
    rows="5" 
    cols="30"
></textarea>
```

## Lista desplegable

```html
<select>
    <option value="html">HTML</option>
    <option value="css">CSS</option>
    <option value="js">JavaScript</option>
</select>
```

---

# 📦 Contenedores

## `<div>`

`div` es un contenedor genérico de tipo bloque.

```html
<div>
    <h2>Mi sección</h2>
    <p>Contenido.</p>
</div>
```

Es muy utilizado junto con CSS.

---

## `<span>`

`span` es un contenedor genérico **en línea**.

```html
<p>
    Este texto tiene una 
    <span>parte especial</span>.
</p>
```

Es útil para aplicar estilos o manipular una parte específica del contenido.

---

# 🧭 Etiquetas semánticas

Las etiquetas semánticas indican qué función cumple cada sección.

```text
<header>
    Encabezado
</header>

<nav>
    Navegación
</nav>

<main>
    Contenido principal

    <section>
        Sección
    </section>

    <article>
        Artículo independiente
    </article>

    <aside>
        Contenido complementario
    </aside>
</main>

<footer>
    Pie de página
</footer>
```

## Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<header>` | Encabezado |
| `<nav>` | Navegación |
| `<main>` | Contenido principal |
| `<section>` | Sección temática |
| `<article>` | Contenido independiente |
| `<aside>` | Contenido complementario |
| `<footer>` | Pie de página |

### ¿Por qué utilizarlas?

Las etiquetas semánticas ayudan a:

- Organizar el código.
- Mejorar la accesibilidad.
- Facilitar el mantenimiento.
- Ayudar a los buscadores a comprender la estructura.

---

# 🎵 Multimedia

## Audio

```html
<audio controls>
    <source src="musica.mp3" type="audio/mpeg">
    Tu navegador no soporta audio.
</audio>
```

## Video

```html
<video controls width="600">
    <source src="video.mp4" type="video/mp4">
    Tu navegador no soporta video.
</video>
```

## YouTube mediante `iframe`

```html
<iframe
    width="560"
    height="315"
    src="https://www.youtube.com/embed/VIDEO_ID"
    title="Video de YouTube"
    allowfullscreen>
</iframe>
```

---

# 💬 Comentarios

Los comentarios no aparecen visualmente en la página.

```html
<!-- Este es un comentario -->
```

También pueden ocupar varias líneas:

```html
<!--
    Este comentario
    ocupa varias líneas.
-->
```

Son útiles para documentar el código.

---

# 🔤 Caracteres especiales

HTML utiliza entidades para representar algunos caracteres.

| Código | Resultado |
|---|---|
| `&lt;` | `<` |
| `&gt;` | `>` |
| `&amp;` | `&` |
| `&quot;` | `"` |
| `&copy;` | © |
| `&nbsp;` | Espacio no separable |

Ejemplo:

```html
<p>5 &lt; 10</p>
```

---

# 🎨 Conectar HTML con CSS

La forma recomendada es utilizar un archivo CSS externo.

### HTML

```html
<head>
    <link rel="stylesheet" href="styles.css">
</head>
```

### CSS

```css
body {
    font-family: Arial, sans-serif;
}

h1 {
    color: blue;
}
```

También existe el CSS interno:

```html
<style>
    h1 {
        color: blue;
    }
</style>
```

Y el CSS en línea:

```html
<h1 style="color: blue;">Título</h1>
```

Para proyectos reales, normalmente se prefiere un **archivo CSS externo**.

---

# ⚡ Conectar HTML con JavaScript

Se puede enlazar un archivo JavaScript mediante:

```html
<script src="script.js"></script>
```

Por ejemplo:

```html
<body>

    <button id="boton">Haz clic</button>

    <script src="script.js"></script>

</body>
```

---

# 🆔 `id` vs `class`

Esta diferencia es fundamental.

## `id`

Identifica normalmente un elemento específico:

```html
<h1 id="titulo-principal">Mi página</h1>
```

En CSS:

```css
#titulo-principal {
    color: red;
}
```

## `class`

Permite aplicar características a varios elementos:

```html
<p class="destacado">Texto 1</p>
<p class="destacado">Texto 2</p>
```

En CSS:

```css
.destacado {
    font-weight: bold;
}
```

### Regla rápida

```text
id    → identificación específica
class → grupo de elementos
```

---

# 📌 Etiquetas HTML esenciales

Esta es una lista rápida para memorizar:

| Etiqueta | Uso |
|---|---|
| `<html>` | Documento HTML |
| `<head>` | Información del documento |
| `<title>` | Título de la pestaña |
| `<body>` | Contenido visible |
| `<h1>`–`<h6>` | Títulos |
| `<p>` | Párrafo |
| `<a>` | Enlace |
| `<img>` | Imagen |
| `<ul>` | Lista desordenada |
| `<ol>` | Lista ordenada |
| `<li>` | Elemento de lista |
| `<table>` | Tabla |
| `<tr>` | Fila |
| `<th>` | Encabezado de tabla |
| `<td>` | Celda |
| `<form>` | Formulario |
| `<input>` | Campo de entrada |
| `<textarea>` | Texto multilínea |
| `<select>` | Lista desplegable |
| `<option>` | Opción |
| `<button>` | Botón |
| `<div>` | Contenedor de bloque |
| `<span>` | Contenedor en línea |
| `<header>` | Encabezado |
| `<nav>` | Navegación |
| `<main>` | Contenido principal |
| `<section>` | Sección |
| `<article>` | Artículo |
| `<aside>` | Contenido adicional |
| `<footer>` | Pie de página |
| `<br>` | Salto de línea |
| `<hr>` | Separación temática |
| `<strong>` | Importancia |
| `<em>` | Énfasis |
| `<audio>` | Audio |
| `<video>` | Video |
| `<iframe>` | Contenido incrustado |

---

# 🧱 Ejemplo completo

A continuación se muestra una página sencilla utilizando varios de los conceptos anteriores:

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Mi primera página</title>

    <link rel="stylesheet" href="styles.css">
</head>

<body>

    <header>
        <h1>Mi página web</h1>

        <nav>
            <a href="#inicio">Inicio</a>
            <a href="#sobre-mi">Sobre mí</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>

    <main>

        <section id="inicio">
            <h2>Bienvenido</h2>

            <p>
                Esta es mi primera página creada utilizando HTML5.
            </p>

            <img 
                src="imagen.jpg"
                alt="Imagen de ejemplo"
                width="400"
            >
        </section>

        <section id="sobre-mi">
            <h2>Sobre mí</h2>

            <p>
                Estoy aprendiendo desarrollo web.
            </p>

            <h3>Mis tecnologías</h3>

            <ul>
                <li>HTML</li>
                <li>CSS</li>
                <li>JavaScript</li>
            </ul>
        </section>

        <section id="contacto">
            <h2>Contacto</h2>

            <form>

                <label for="nombre">Nombre:</label>
                <input
                    type="text"
                    id="nombre"
                    name="nombre"
                    required
                >

                <br><br>

                <label for="correo">Correo:</label>
                <input
                    type="email"
                    id="correo"
                    name="correo"
                    required
                >

                <br><br>

                <label for="mensaje">Mensaje:</label>

                <br>

                <textarea
                    id="mensaje"
                    name="mensaje"
                    rows="5"
                ></textarea>

                <br><br>

                <button type="submit">
                    Enviar
                </button>

            </form>
        </section>

    </main>

    <footer>
        <p>&copy; 2026 Mi página web</p>
    </footer>

</body>

</html>
```

---

# 🧠 Conceptos que debes dominar primero

Si estás empezando, aprende en este orden:

```text
1. Estructura HTML
        ↓
2. Etiquetas básicas
        ↓
3. Atributos
        ↓
4. Enlaces e imágenes
        ↓
5. Listas y tablas
        ↓
6. Formularios
        ↓
7. Div y Span
        ↓
8. Etiquetas semánticas
        ↓
9. CSS
        ↓
10. JavaScript
```

No es necesario memorizar todas las etiquetas. Lo importante es **entender la estructura y saber buscar la etiqueta adecuada cuando la necesites**.

---

# 🛠️ Estructura recomendada de un proyecto

Una estructura sencilla puede ser:

```text
mi-proyecto/
│
├── index.html
├── styles.css
├── script.js
│
└── img/
    ├── logo.png
    └── foto.jpg
```

### `index.html`

Contiene la estructura.

### `styles.css`

Contiene los estilos.

### `script.js`

Contiene la lógica e interactividad.

### `img/`

Contiene las imágenes.

---

# ✅ Buenas prácticas

### 1. Utiliza HTML semántico

Prefiere:

```html
<header>
<nav>
<main>
<section>
<article>
<footer>
```

cuando corresponda, en lugar de utilizar `<div>` para absolutamente todo.

### 2. Utiliza `alt` en las imágenes

```html
<img src="foto.jpg" alt="Descripción de la imagen">
```

### 3. Utiliza etiquetas correctamente anidadas

Correcto:

```html
<p>
    <strong>Texto importante</strong>
</p>
```

Evita estructuras mal cerradas o cruzadas.

### 4. Mantén el código organizado

Usa indentación:

```html
<section>
    <h2>Título</h2>

    <p>
        Contenido.
    </p>
</section>
```

### 5. Utiliza nombres descriptivos

Mejor:

```html
<div class="producto-principal">
```

que:

```html
<div class="caja1">
```

### 6. Evita abusar de `style`

En lugar de:

```html
<h1 style="color: red;">
```

es preferible utilizar CSS externo:

```html
<h1 class="titulo">Mi título</h1>
```

```css
.titulo {
    color: red;
}
```

---

# 🚀 Resumen rápido

HTML se puede entender como una estructura de elementos:

```text
HTML
│
├── HEAD
│   ├── META
│   ├── TITLE
│   └── LINK → CSS
│
└── BODY
    │
    ├── HEADER
    ├── NAV
    ├── MAIN
    │   ├── SECTION
    │   ├── ARTICLE
    │   └── ASIDE
    │
    └── FOOTER
```

La idea fundamental es:

> **HTML estructura, CSS diseña y JavaScript hace interactiva la página.**

---

## 📖 Mini chuleta

```html
<!-- Comentario -->

<h1>Título</h1>
<p>Párrafo</p>

<a href="pagina.html">Enlace</a>

<img src="imagen.jpg" alt="Descripción">

<ul>
    <li>Elemento</li>
</ul>

<ol>
    <li>Elemento</li>
</ol>

<div>Contenedor</div>
<span>Texto</span>

<form>
    <label for="nombre">Nombre</label>
    <input type="text" id="nombre">

    <button type="submit">Enviar</button>
</form>

<header>Encabezado</header>
<nav>Navegación</nav>
<main>Contenido principal</main>
<section>Sección</section>
<article>Artículo</article>
<aside>Contenido adicional</aside>
<footer>Pie de página</footer>
```

---

**HTML5 — Guía básica de referencia**

*Ideal para comenzar a construir páginas web y posteriormente incorporar CSS, Bootstrap y JavaScript.*
