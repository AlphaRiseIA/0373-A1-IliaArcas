
# Introducción a HTML

HTML (HyperText Markup Language) es el lenguaje de marcado estándar para crear páginas web. **Lenguaje más importante de Internet** dado que sin HTML no se vería nada en el navegador.

HTML define **la estructura y el contenido** (es decir, si hay una imagen, una lista de elementos, un enlace, un párrafo, un titular, etc.) de las páginas web mediante etiquetas. Es muy adaptable, tiene una estructura lógica y es fácil de entender e interpretar. **Describe el contenido**.

No se dedica a cómo se interactúa con el contenido (Javascript, PHP, etc.) ni a la presentación o estilización del contenido (para eso tenemos CSS).

Los elementos **HTML** son los bloques de construcción de las páginas HTML. HTML fue desarrollado en 1991 por **Tim Berners-Lee**.

Cada elemento HTML está delimitado por etiquetas, como `<body>`, `<head>`, `<p>`, `<h1>`, etc.

---

## Significado de HTML

- **HyperText**: Significa hipertexto, un texto que enlaza con otros contenidos (texto o archivos). Es la base del funcionamiento de la web tal y como la conocemos, con páginas y recursos interconectados.
- **Markup**: Significa marca o etiqueta. Todas las páginas web se construyen en base a etiquetas, desde las primeras versiones hasta HTML5. Ejemplo de etiqueta: `<p>HOLA</p>`.
- **Language**: Es un lenguaje con normas y estructura para definir la estructura y contenido de una web. **No es un lenguaje de programación**, ya que carece de bucles, condiciones, funciones, etc.

---

## Elementos HTML

HTML no es un lenguaje de programación; es un lenguaje de marcado que define la estructura de su contenido. Los elementos se usan para encerrar diferentes partes del contenido, etiquetándolo para que el navegador sepa cómo mostrarlo.

### Componentes del elemento
- **Etiqueta de apertura**: Consiste en el nombre del elemento, encerrado por `< >`.
- **Etiqueta de cierre**: Igual que la apertura, pero con una barra `/` antes del nombre.
- **Contenido**: Texto o información dentro del elemento.
- **Elemento**: Conjunto de la etiqueta de apertura, cierre y contenido.

---

## Atributos

Los elementos pueden tener **atributos** que proporcionan información adicional sobre un elemento. Estos atributos no aparecen en el contenido visual.

### Ejemplo de Atributos
```html
<p class="editor-note">Mi gato es muy gruñón</p>
```
- **Atributo**: El nombre del atributo seguido de un signo `=`.
- **Valor**: El valor del atributo encerrado entre comillas.

**Reglas para los atributos**:
1. Un espacio entre el atributo y el nombre del elemento.
2. Se especifican en la etiqueta de apertura.
3. Algunos elementos como `<img>` no tienen contenido ni etiqueta de cierre y se llaman **elementos vacíos**.

---

## Estructura básica de un archivo HTML

Una página HTML básica contiene:
- **DOCTYPE**: Declara el tipo de documento.
- **html**: Encierra todo el contenido.
- **head**: Contiene metadatos como estilos y scripts.
- **body**: Contiene el contenido visible de la página.

### Ejemplo de estructura básica

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mi página de prueba</title>
    <link rel="icon" href="favicon.png">
  </head>
  <body>
    <img src="images/firefox-icon.png" alt="Mi imagen de prueba">
  </body>
</html>
```

---

## Detalles del Head

- **Juego de caracteres**: `<meta charset="utf-8">` para todos los caracteres globales.
- **Descripción y keywords**: Metadatos importantes para SEO.
- **Título**: Se muestra en la pestaña del navegador.
- **Favicon**: Icono del sitio.
- **Hojas de estilo y scripts**: Para diseño y funcionalidad.
- **CSS en línea**: Definir estilos básicos.

---

## Elementos de bloque y línea

Dentro del `<body>`, se deben incluir todos los elementos visibles de la web:

- **Elementos de bloque**: Separan contenido en bloques. Ejemplos: `<h1>`, `<p>`, `<blockquote>`, `<div>`.
- **Elementos de línea**: Se muestran en línea. Ejemplos: `<em>`, `<strong>`, `<q>`, `<span>`, `<cite>`.

---

## Resumen de Normas Básicas de Etiquetas HTML

1. **Etiquetas**: Normalmente vienen en pares con una apertura y cierre (`<p>` y `</p>`).
2. **Etiquetas vacías**: No tienen cierre, como `<img>`, `<br>`, `<input>`.
3. **Anidamiento**: Las etiquetas deben anidarse correctamente.
4. **Atributos**: Se especifican en la etiqueta de apertura con el formato `nombre="valor"`.

**Recomendación**: Escribir etiquetas y atributos en minúsculas.

---

# Legibilidad y Organización del Código

La legibilidad del código fuente es la claridad con la que está codificado, en el sentido de que un ser humano
sea capaz de entenderlo de manera fácil y rápida. **Es fundamental que el código fuente HTML que
generemos sea legible**.

Debemos pensar que normalmente no trabajaremos solos, y hacer que lo que hemos desarrollado sea legible
puede ayudar a aquellos que trabajan con nuestro documento a entender qué hemos hecho y por qué lo hemos
hecho. Incluso, suponiendo que el documento creado solo será modificado por nosotros, la legibilidad también
es indispensable para recordar todo lo que hemos hecho.

**Entenderemos por organización del código fuente la estructuración de la aplicación web en varios
archivos, así como la clasificación de estos archivos en los directorios que sean necesarios.**

## Técnicas para Legibilidad
- Los comentarios.
- La indentación del código.
- La organización de los archivos.

---

## Comentarios

En un documento HTML, podemos poner anotaciones que no se verán reflejadas cuando se mire la web con
el navegador, pero que son útiles para el desarrollador web.

### Sintaxis de Comentarios
```html
<!-- comentario -->
```

Es muy importante comentar el código fuente, sobre todo si se trata de un documento muy largo.

**Ejemplo:**
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8"/>
    <title>Título de la web</title>
  </head>
  <body>
    <!-- Cabecera -->
    <!-- Menú de navegación -->
    <!-- Columna lateral con enlaces interesantes para el usuario -->
    <!-- Sección principal con artículos -->
    <!-- Pie de página -->
  </body>
</html>
```

---

## Indentación del Código

El código HTML está lleno de etiquetas que se abren y cierran. El navegador web interpretará este
código sin necesidad de saltos de página o tabuladores, pero los seres humanos necesitamos que esté
organizado con saltos de línea e indentaciones.

**Técnica de Indentación:**
- Todo el contenido entre una etiqueta de inicio y su etiqueta de cierre debe estar indentado.

**Ejemplo:**
```html
<div>
  <p>Esto es el contenido de un párrafo</p>
</div>
```

---

## Organización de Archivos

Cuando la aplicación web es grande, tendrá varios archivos con extensión `.html`, hojas de estilo `.css`, imágenes, videos, etc. **Si tenemos todos estos archivos mezclados, nuestra aplicación web tenderá al caos.**

Es recomendable crear un directorio principal y subdirectorios para organizar todo.

**Estructura de Directorios:**
```
web/
  ├── imatges/
  │   ├── img1.png
  │   ├── img2.jpg
  ├── videos/
  ├── audios/
  ├── css/
  │   └── estil.css
  ├── index.html
  ├── seccion1.html
  └── seccion2.html
```

---

## Etiquetas Básicas de HTML

### Encabezados
```html
<h1>...</h6>
```
- Permiten especificar encabezados. **Son elementos de bloque.**

### Párrafos
```html
<p>
```
- Se utilizan para párrafos de texto. **Son elementos de bloque.**

### Salto de Línea
```html
<br>
```
- Agrega un salto de línea.

### Separador de Línea
```html
<hr>
```
- Agrega una línea horizontal divisoria.

### Énfasis
```html
<em>, <strong>
```
- Se usan para destacar texto.

### Contenedor en Línea
```html
<span>
```
- Agrupa partes de texto en línea.

---

## Enlaces
```html
<a href="...">
```
- Usamos el atributo `href` para indicar el destino.

### Ejemplo de Enlace Externo
```html
<p><a href="https://m.joan23.fje.edu/" title="Joan XXIII">Jesuites Bellvitge – Joan XXIII</a></p>
```

### Ejemplo de Enlace Local
```html
<div id="menu">
  <a href="index.html" title="Inicio">Inicio</a>
</div>
```

---

## Listas

### Listas Desordenadas
```html
<ul>
```
- Usadas cuando el orden no es relevante.

### Listas Ordenadas
```html
<ol>
```
- Usadas cuando el orden importa.

### Elementos de Lista
```html
<li>
```
- Cada ítem de la lista se coloca dentro de `<li>`.

---

## Rutas en HTML

### Ruta Absoluta
```html
<img src="https://www.example.com/images/logo.png" alt="Logo de Example">
```

### Ruta Relativa
```html
<img src="images/logo.png" alt="Logo de Mi Sitio">
```

---

## Imágenes
```html
<img src="..." alt="...">
```
- La etiqueta `<img>` no tiene cierre. Usamos `src` para la ubicación y `alt` para texto alternativo.

### Ejemplo
```html
<img src="media/logo.png" alt="Logo de la web" />
```

---

<!-- Estos apuntes han sido inspirados en los apuntes de las diapositivas mostradas en clase -->
