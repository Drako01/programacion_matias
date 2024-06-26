# ¡Creación de una página HTML usando buenas prácticas!


## Guía para Crear una Página HTML Usando Buenas Prácticas

## Introducción

Este documento tiene como objetivo guiarte a través del proceso de creación de una página HTML básica utilizando buenas prácticas. HTML (HyperText Markup Language) es el lenguaje estándar para crear páginas web y es fundamental para cualquier desarrollador web.

## Requisitos Previos

No se requieren conocimientos previos para seguir esta guía. Sin embargo, un editor de texto (como Visual Studio Code, Sublime Text o Atom) y un navegador web (como Google Chrome, Firefox o Safari) serán necesarios.

## Estructura Básica de un Documento HTML

Cada documento HTML debe seguir una estructura básica. Aquí tienes un ejemplo de la estructura mínima de una página HTML:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Primera Página HTML</title>
</head>
<body>
    <header>
        <h1>Bienvenido a Mi Página</h1>
    </header>
    <main>
        <p>Este es un párrafo de ejemplo.</p>
    </main>
    <footer>
        <p>&copy; 2024 Mi Nombre</p>
    </footer>
</body>
</html>
```

### Descripción de la Estructura

1. `<!DOCTYPE html>`: Declara el tipo de documento como HTML5.
2. `<html lang="es">`: La etiqueta `<html>` envuelve todo el contenido de la página. El atributo `lang="es"` define el idioma de la página como español.
3. `<head>`: Contiene metadatos sobre el documento, como el juego de caracteres (`charset`) y el título (`title`) que se muestra en la pestaña del navegador.
4. `<meta charset="UTF-8">`: Define la codificación de caracteres como UTF-8.
5. `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Hace que el diseño sea adaptable a diferentes tamaños de pantalla.
6. `<title>`: Define el título de la página.
7. `<body>`: Contiene el contenido visible de la página.

## Buenas Prácticas

### 1. **Uso de Etiquetas Semánticas**

Utiliza etiquetas HTML semánticas como `<header>`, `<main>`, `<footer>`, `<article>`, y `<section>`. Estas etiquetas ayudan a mejorar la accesibilidad y el SEO de tu página.

### 2. **Organización del Código**

Mantén tu código limpio y organizado. Utiliza la indentación y espacios en blanco para mejorar la legibilidad. Aquí tienes un ejemplo de una buena práctica:

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ejemplo de Buenas Prácticas</title>
</head>
<body>
    <header>
        <h1>Encabezado Principal</h1>
    </header>
    <main>
        <section>
            <h2>Sección 1</h2>
            <p>Contenido de la primera sección.</p>
        </section>
        <section>
            <h2>Sección 2</h2>
            <p>Contenido de la segunda sección.</p>
        </section>
    </main>
    <footer>
        <p>&copy; 2024 Mi Nombre</p>
    </footer>
</body>
</html>
```

### 3. **Comentarios**

Utiliza comentarios para explicar secciones de tu código. Esto es útil para ti y para otros desarrolladores que puedan trabajar en tu código en el futuro.

```html
<!-- Esto es un comentario -->
```

### 4. **Accesibilidad**

Asegúrate de que tu página sea accesible para todos los usuarios, incluyendo aquellos con discapacidades. Utiliza atributos como `alt` en las imágenes y `aria` en elementos interactivos.

```html
<img src="imagen.jpg" alt="Descripción de la imagen">
```

### 5. **SEO (Optimización para Motores de Búsqueda)**

Incluye metaetiquetas relevantes y usa etiquetas de encabezado (`<h1>`, `<h2>`, etc.) de manera apropiada para mejorar el SEO de tu página.

```html
<meta name="description" content="Descripción de mi página web">
```

## Recursos Adicionales

- [Documentación de MDN Web Docs](https://developer.mozilla.org/es/docs/Web/HTML)
- [Curso de HTML en W3Schools](https://www.w3schools.com/html/)
- [Guía de Accesibilidad Web](https://www.w3.org/WAI/tips/developing/)

## Conclusión

Siguiendo esta guía, deberías ser capaz de crear una página HTML básica que siga buenas prácticas. Continúa explorando y aprendiendo más sobre HTML y otras tecnologías web para mejorar tus habilidades como desarrollador.

---


# Incluyendo CSS a nuestro proyecto - Clase 02

#### Objetivos de la clase:
- Comprender la sintaxis de CSS.
- Incluir CSS en nuestro Proyecto.
- Conocer el uso de medidas, colores, fuentes y fondos en CSS.

---

### Glosario

**Listas:** HTML permite agrupar elementos que tienen más significado de forma conjunta. Aunque cada palabra por separado tiene sentido, de forma conjunta constituyen el menú de navegación de la página, por lo que su significado conjunto es mayor que por separado. Esto se denomina listas.

**Tablas:** Son un conjunto de celdas organizadas, dentro del cual es posible alojar distintos contenidos. Sirven para representar información tabulada, en filas y columnas.

**Formularios:** Son etiquetas donde el usuario ingresará o seleccionará valores, que serán enviados a un archivo encargado de procesar la información.

**Enlaces:** También conocidos como links o anchors, se utilizan para relacionar partes del mismo documento. Por defecto, se visualizan azules y subrayados.

---

### Mapa de Conceptos

- Atributos
- Bases de CSS
- Propiedades
- Class
- Reglas sintácticas
- Sintaxis de CSS
- Padres e hijos
- ¿Qué es CSS?
- ID

---

### Temario

1. Primeros pasos con HTML
2. Incluyendo CSS a nuestro proyecto
3. CSS + Box Modeling

---

### Bases de CSS

**CSS (Cascading Style Sheets):** Es un lenguaje web para aplicar formato visual (color, tamaño, separación y ubicación) al HTML. Permite cambiar por completo el aspecto de cualquier etiqueta HTML.

---

### Sintaxis de CSS

```css
selector {
   propiedad1: valor;
   propiedad2: valor;
}

h1 {
   color: red;
}
```

**Reglas sintácticas:**
1. Cada declaración CSS está formada por un juego de pares propiedad:valor.
2. No se ve afectado por el espacio en blanco. Las propiedades se pueden escribir de corrido o una debajo de la otra.
3. Siempre que la propiedad represente un número, el valor debe indicar en qué unidad se expresa.

---

### Padres e Hijos

Cuando tienes una etiqueta "dentro" de otra, aplicas el concepto de padres e hijos. Esto permite agregar atributos específicos a “hijos” sin alterar los del “padre”. 

```html
<section>
    <article> 
        <h2>Título</h2>
        <p>Lorem ipsum dolor sit amet...</p>
    </article>
</section>
```

---

### Insertar CSS en el HTML

**Forma externa:**
```html
<link rel="stylesheet" href="archivo.css" />
```

**Forma interna:**
```html
<style>
    /* comentario de CSS dentro de esta etiqueta va el código CSS */
</style>
```

**Forma inline (no recomendable):**
```html
<h2 style="color: red;">H2 con formato CSS</h2>
```

---

### Class

**Desde CSS:**
```css
.bordesRedondeados {
  /* código CSS */
}
```

**En HTML:**
```html
<img src="" class="bordesRedondeados" />
```

Puedes aplicar más de una clase a cada etiqueta separada por un espacio:
```html
<img src="" class="bordesRedondeados imgChica"/>
```

---

### Atributo ID

**Desde CSS:**
```css
#productos {
  /* código CSS */
}
```

**En HTML:**
```html
<section id="productos"></section>
```

### Class vs ID

- **ID:** Nombrar secciones, divisiones de código (único por documento).
- **Class:** Especificar diseño aparte del código (puede repetirse).

```html
<section id="prod">
  <article class="rojo"></article>
  <article class="rojo"></article>
</section>
```

---

### Herencia y Cascada

**Herencia:** Los elementos hijos heredan propiedades del elemento padre, a menos que tengan estilos específicos aplicados.

```css
div {
   color: red;
}

<div>
   <p>Este párrafo quedará en rojo por herencia</p>
</div>
```

**Cascada:** El navegador lee de arriba hacia abajo. La última declaración prevalece.

```css
p {
   color: red;
}

p {
   color: green;
}
```

### Precedencia de Declaraciones

1. **ID:** Pisan cualquier otra regla.
2. **Class:** Sobreescriben las reglas de etiqueta pero no las de ID.
3. **Etiquetas:** Tienen la menor precedencia.

```css
ID > Class > Etiquetas
```

---

### Estilos Inline

Los estilos inline sobrescriben cualquier estilo de las páginas externas de CSS y tienen la mayor especificidad.

```html
<p style="color: red">Párrafo rojo</p>
```

---

### Importancia de los Selectores

- Estilo aplicado a la Etiqueta.
- Estilo aplicado a la Class.
- Estilo aplicado al ID.
- Estilo aplicado Inline.

### !important

La declaración `!important` corta la precedencia. Se escribe después del valor de la propiedad CSS que se quiere convertir en la más importante. Se recomienda no abusar de esta práctica.

```css
color: red !important;
```

### Reset CSS

Los reset CSS unifican estilos entre diferentes navegadores.

```css
* {
   margin: 0;
   padding: 0;
}
```

### Primeras Propiedades

**Propiedad: color**
Mediante esta propiedad se puede agregar color a los textos del sitio.

Valores comunes:
- Nombre del color (ej: red).
- Hexadecimal (ej: #ffffff).
- RGB (ej: rgb(50, 212, 227)).

### Estilos de Texto

**FONT-STYLE:**

```css
.normal {
   font-style: normal;
}

.italica {
   font-style: italic;
}
```

**FONT-WEIGHT:**

```css
.normal {
   font-weight: normal;
}

.negrita {
   font-weight: bold;
}
```

---

## [Autor: Alejandro Di Stefano](https://github.com/Drako01)


