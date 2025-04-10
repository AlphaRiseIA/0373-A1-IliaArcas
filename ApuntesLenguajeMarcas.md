# APUNTES DE LENGUAJE DE MARCAS

## ÍNDICE
1. [GitHub](#github)
2. [Markdown](#markdown)
3. [HTML](#html)
4. [CSS](#css)
5. [Flexbox](#flexbox)
6. [Responsive Design](#responsive-design)
7. [XML](#xml)

---

## GITHUB

GitHub es una plataforma basada en la web que usa el sistema de control de versiones Git. Se utiliza principalmente para alojar y gestionar proyectos de software, permitiendo la colaboración entre desarrolladores. Es una herramienta esencial para cualquier programador moderno.


### ¿Qué es GitHub?
GitHub es un portal que permite alojar proyectos de desarrollo en la nube, usar control de versiones con Git y colaborar con otros usuarios. Los repositorios pueden ser públicos o privados, y cada cambio en ellos se registra mediante un **commit**. Es posible sincronizar repositorios locales con la nube usando comandos de Git.

- GitHub permite trabajar en equipo compartiendo código en la nube.
- Los repositorios públicos pueden ser copiados por otros, pero **no modificados directamente** sin permisos.
- Cada cambio se guarda como un **commit**, una versión concreta de los archivos en un punto del tiempo.
- GitHub permite colaborar en proyectos ajenos usando **forks** y **pull requests**.

### Crear una cuenta en GitHub
Registrarse en [GitHub](https://github.com) para poder crear o colaborar en repositorios.

### Repositorios y comandos esenciales
- `git init`: Inicializa un repositorio en local.
- `git branch -m "rama"`: Cambia el nombre de la rama.
- `git add archivo`: Añade archivo al área de preparación.
- `git add .`: Añade todos los archivos modificados al área de preparación.
- `git commit -m "mensaje"`: Registra los cambios.
- `git push origin main`: Sube los cambios al repositorio remoto.
- `git remote add origin URL`: Asocia el repositorio local con el remoto.
- `git branch`: Muestra todas las ramas del proyecto.


### ¿Qué es GitHub?
GitHub es un portal que permite alojar proyectos de desarrollo en la nube, usar control de versiones con Git y colaborar con otros usuarios. Los repositorios pueden ser públicos o privados, y cada cambio en ellos se registra mediante un **commit**. Es posible sincronizar repositorios locales con la nube usando comandos de Git.

### Crear una cuenta en GitHub
Registrarse en [GitHub](https://github.com) para poder crear o colaborar en repositorios.

### Repositorios y comandos esenciales
- `git init`: Inicializa un repositorio en local.
- `git branch -m "rama"`: Cambia el nombre de la rama.
- `git add archivo`: Añade archivo al área de preparación.
- `git commit -m "mensaje"`: Registra los cambios.
- `git push origin main`: Sube los cambios al repositorio remoto.
- `git remote add origin URL`: Asocia el repositorio local con el remoto.

---



## MARKDOWN

Markdown es un lenguaje de marcado ligero que permite aplicar formato a texto de manera sencilla y legible. Se usa mucho en documentos README, blogs, documentación técnica y foros. Su simplicidad lo hace ideal para crear contenido estructurado sin necesidad de herramientas complejas.


### Detalles adicionales sobre Markdown

- Puedes usar tanto `*` como `_` para marcar **negrita** y *cursiva*, lo que importa es la cantidad de caracteres (`*`, `**`, `***` o `_`, `__`, `___`).
- Para mostrar bloques de código puedes usar triple acento grave (```) o sangría de 4 espacios.
- Las imágenes deben estar ubicadas en el mismo repositorio local para que se muestren correctamente si son locales.


### Encabezados
Markdown permite jerarquizar texto con `#`, `##`, `###`, etc.

### Estilos de texto
- *Cursiva*: `_texto_` o `*texto*`
- **Negrita**: `**texto**`
- ***Ambos***: `***texto***`

### Listas
- Ordenadas: `1. Item`
- Desordenadas: `- Item`

### Código
```
    ```
    <html>
        <body>Hello</body>
    </html>
    ```
```

### Enlaces e imágenes
- `[Texto](URL)`
- `![Texto alternativo](ruta "Título opcional")`

### Tablas
```
| Título 1 | Título 2 |
|----------|----------|
| Dato 1   | Dato 2   |
```

---

## HTML

HTML (HyperText Markup Language) es el lenguaje de marcado estándar para crear páginas web. Su función es estructurar la información, dividiéndola en elementos como encabezados, párrafos, enlaces, imágenes, tablas, etc. Es el pilar fundamental del desarrollo web.


### Detalles adicionales sobre HTML

#### Elementos semánticos de HTML5
HTML5 introdujo etiquetas semánticas que indican la finalidad del contenido, mejorando la accesibilidad y el SEO:
- `<header>`: Encabezado del sitio o sección.
- `<footer>`: Pie de página.
- `<nav>`: Navegación.
- `<article>`: Contenido independiente.
- `<section>`: División temática.

#### Formularios avanzados
Los formularios permiten recoger datos del usuario. Algunos atributos y elementos adicionales:
- `fieldset` y `legend`: Agrupan elementos de un formulario con un título.
- `select` y `option`: Para desplegables.
- `radio` y `checkbox`: Selecciones simples o múltiples.

```html
<form>
  <fieldset>
    <legend>Elige tu idioma</legend>
    <input type="radio" name="idioma" value="es"> Español
    <input type="radio" name="idioma" value="ca"> Catalán
  </fieldset>
</form>
```

#### Tablas HTML avanzadas
Atributos especiales:
- `colspan`: Hace que una celda ocupe varias columnas.
- `rowspan`: Hace que una celda ocupe varias filas.
- `bgcolor`: Cambia el color de fondo (aunque se recomienda usar CSS).


### ¿Qué es HTML?
HTML (HyperText Markup Language) es un lenguaje de marcado usado para estructurar el contenido de las páginas web. Fue creado por Tim Berners-Lee.

### Estructura básica
```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <title>Mi página</title>
  </head>
  <body>
    Contenido visible
  </body>
</html>
```

### Elementos y atributos
Los elementos pueden tener atributos como `id`, `class`, `href`, etc. Algunos como `<img>` o `<br>` no tienen etiqueta de cierre.

### Tipos de elementos
- De bloque: `<div>`, `<p>`, `<h1>`, etc.
- En línea: `<span>`, `<strong>`, `<em>`, etc.

### Enlaces e imágenes
```html
<a href="https://example.com">Visita</a>
<img src="logo.png" alt="Logo">
```

### Formularios
```html
<form>
  <input type="text" name="nombre" placeholder="Tu nombre">
  <button type="submit">Enviar</button>
</form>
```

### Organización y legibilidad
- Indentación
- Comentarios: `<!-- comentario -->`
- Estructura de carpetas recomendada

---

## CSS

CSS (Cascading Style Sheets) se usa para definir la presentación visual de un documento HTML. Permite aplicar estilos como colores, márgenes, alineación, fuentes, animaciones, entre otros. Con CSS se separa el contenido del diseño, facilitando la mantenibilidad del código.


### Detalles adicionales sobre CSS

#### Comentarios en CSS
Se hacen con `/* comentario */` y permiten documentar partes del código.

#### Herencia y cascada
CSS aplica estilos según un orden de prioridad:
1. Estilos inline
2. Estilos en el head
3. Estilos en archivos externos
Además, los estilos más específicos y los definidos más abajo sobrescriben los anteriores.

#### `!important`
Si se usa `!important` en una regla, esta tendrá prioridad sobre cualquier otra, aunque no se recomienda abusar de él.

```css
p {
  color: red !important;
}
```


### ¿Qué es CSS?
Hojas de estilo en cascada que permiten separar contenido y presentación.

### Tipos de CSS
- Inline: `style=""` en una etiqueta HTML.
- Interno: dentro de `<style>` en el `<head>`.
- Externo: archivo `.css` vinculado con `<link>`.

### Selectores
- Básicos: `p`, `.clase`, `#id`
- Avanzados: `*`, `[type="text"]`, `div > p`, `p::first-letter`, `a:hover`

### Sintaxis básica
```css
p {
  color: red;
  font-size: 16px;
}
```

---

## FLEXBOX

Flexbox es un módulo de CSS diseñado para distribuir espacio y alinear ítems dentro de un contenedor, incluso cuando su tamaño es dinámico. Facilita la creación de diseños modernos, centrados, adaptables y responsivos sin complicadas estructuras.


### Tips adicionales sobre Flexbox

- `align-self` permite que un ítem individual sobrescriba la alineación definida por el contenedor.
- `flex-wrap` permite que los elementos se ajusten a múltiples líneas:
```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```


### ¿Qué es Flexbox?
Modelo de diseño en CSS para crear layouts flexibles y responsivos.

### Propiedades del contenedor
- `display: flex;`
- `flex-direction`, `justify-content`, `align-items`

### Propiedades de los ítems
- `flex-grow`, `flex-shrink`, `flex-basis`

---

## RESPONSIVE DESIGN

El diseño responsive permite que una web se vea correctamente en cualquier dispositivo, ya sea ordenador, tablet o móvil. Se logra con técnicas como media queries, rejillas fluidas y contenido flexible. Es imprescindible hoy en día por el uso masivo de móviles.


### Detalles adicionales sobre diseño responsive

#### Buenas prácticas
- Usar unidades relativas como `%`, `em`, `rem` en lugar de `px`.
- Evitar valores fijos en elementos clave como ancho o alto.
- Usar `max-width: 100%` para hacer que las imágenes se escalen correctamente.

#### Breakpoints comunes
```css
@media (max-width: 1200px) { ... } /* Escritorio */
@media (max-width: 992px) { ... }  /* Tablets grandes */
@media (max-width: 768px) { ... }  /* Tablets */
@media (max-width: 576px) { ... }  /* Móviles */
```


### ¿Qué es Responsive Design?
Técnica para adaptar una web a diferentes dispositivos.

### Media Queries
```css
@media (max-width: 768px) {
  body {
    background-color: green;
  }
}
```

---

## XML

XML (eXtensible Markup Language) es un lenguaje diseñado para almacenar, transportar y estructurar datos. A diferencia de HTML, XML no está orientado a mostrar contenido, sino a representar datos de forma jerárquica y extensible. Es ampliamente usado en configuración y comunicación entre sistemas.


### Características adicionales de XML

- Las etiquetas deben estar siempre cerradas.
- Es sensible a mayúsculas y minúsculas.
- No permite etiquetas abiertas o mal anidadas.
- Requiere una raíz única que contenga todos los nodos hijos.

Ejemplo:
```xml
<libros>
  <libro>
    <titulo>1984</titulo>
    <autor>George Orwell</autor>
  </libro>
</libros>
```


### ¿Qué es XML?
Lenguaje de marcas extensible, diseñado para almacenar y transportar datos.

### Características
- Definición propia de etiquetas.
- Estructura jerárquica.
- Legible por humanos y máquinas.


## CSS

CSS (Cascading Style Sheets) se usa para definir la presentación visual de un documento HTML. Permite aplicar estilos como colores, márgenes, alineación, fuentes, animaciones, entre otros. Con CSS se separa el contenido del diseño, facilitando la mantenibilidad del código.


### Detalles adicionales sobre CSS

#### Comentarios en CSS
Se hacen con `/* comentario */` y permiten documentar partes del código.

#### Herencia y cascada
CSS aplica estilos según un orden de prioridad:
1. Estilos inline
2. Estilos en el head
3. Estilos en archivos externos
Además, los estilos más específicos y los definidos más abajo sobrescriben los anteriores.

#### `!important`
Si se usa `!important` en una regla, esta tendrá prioridad sobre cualquier otra, aunque no se recomienda abusar de él.

```css
p {
  color: red !important;
}
```


### ¿Qué es CSS?
Hojas de estilo en cascada que permiten separar contenido y presentación.

### Tipos de CSS
- Inline: `style=""` en una etiqueta HTML.
- Interno: dentro de `<style>` en el `<head>`.
- Externo: archivo `.css` vinculado con `<link>`.

### Selectores
- Básicos: `p`, `.clase`, `#id`
- Avanzados: `*`, `[type="text"]`, `div > p`, `p::first-letter`, `a:hover`

### Sintaxis básica
```css
p {
  color: red;
  font-size: 16px;
}
```

---

## FLEXBOX

Flexbox es un módulo de CSS diseñado para distribuir espacio y alinear ítems dentro de un contenedor, incluso cuando su tamaño es dinámico. Facilita la creación de diseños modernos, centrados, adaptables y responsivos sin complicadas estructuras.


### Tips adicionales sobre Flexbox

- `align-self` permite que un ítem individual sobrescriba la alineación definida por el contenedor.
- `flex-wrap` permite que los elementos se ajusten a múltiples líneas:
```css
.container {
  display: flex;
  flex-wrap: wrap;
}
```


### ¿Qué es Flexbox?
Modelo de diseño en CSS para crear layouts flexibles y responsivos.

### Propiedades del contenedor
- `display: flex;`
- `flex-direction`, `justify-content`, `align-items`

### Propiedades de los ítems
- `flex-grow`, `flex-shrink`, `flex-basis`

---

## RESPONSIVE DESIGN

El diseño responsive permite que una web se vea correctamente en cualquier dispositivo, ya sea ordenador, tablet o móvil. Se logra con técnicas como media queries, rejillas fluidas y contenido flexible. Es imprescindible hoy en día por el uso masivo de móviles.


### Detalles adicionales sobre diseño responsive

#### Buenas prácticas
- Usar unidades relativas como `%`, `em`, `rem` en lugar de `px`.
- Evitar valores fijos en elementos clave como ancho o alto.
- Usar `max-width: 100%` para hacer que las imágenes se escalen correctamente.

#### Breakpoints comunes
```css
@media (max-width: 1200px) { ... } /* Escritorio */
@media (max-width: 992px) { ... }  /* Tablets grandes */
@media (max-width: 768px) { ... }  /* Tablets */
@media (max-width: 576px) { ... }  /* Móviles */
```


### ¿Qué es Responsive Design?
Técnica para adaptar una web a diferentes dispositivos.

### Media Queries
```css
@media (max-width: 768px) {
  body {
    background-color: green;
  }
}
```

---

## XML

XML (eXtensible Markup Language) es un lenguaje diseñado para almacenar, transportar y estructurar datos. A diferencia de HTML, XML no está orientado a mostrar contenido, sino a representar datos de forma jerárquica y extensible. Es ampliamente usado en configuración y comunicación entre sistemas.


### Características adicionales de XML

- Las etiquetas deben estar siempre cerradas.
- Es sensible a mayúsculas y minúsculas.
- No permite etiquetas abiertas o mal anidadas.
- Requiere una raíz única que contenga todos los nodos hijos.

Ejemplo:
```xml
<libros>
  <libro>
    <titulo>1984</titulo>
    <autor>George Orwell</autor>
  </libro>
</libros>
```


### ¿Qué es XML?
Lenguaje de marcas extensible, diseñado para almacenar y transportar datos.

### Características
- Definición propia de etiquetas.
- Estructura jerárquica.
- Legible por humanos y máquinas.
