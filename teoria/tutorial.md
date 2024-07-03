## Tutorial Básico de HTML y CSS

### Introducción a HTML

HTML (HyperText Markup Language) es el lenguaje estándar para crear páginas web. Utilizamos HTML para estructurar el contenido, como títulos, párrafos, imágenes y enlaces.

#### Estructura Básica de un Documento HTML

Todo documento HTML comienza con la declaración `<!DOCTYPE html>` seguida de elementos `<html>`, `<head>`, y `<body>`. Aquí tienes un ejemplo de la estructura básica:

```html
<!DOCTYPE html>
<html>
<head>
    <title>Título de la Página</title>
</head>
<body>
    <!-- Contenido de la página -->
</body>
</html>
```

### Elementos HTML Básicos

1. **Encabezados**: Se utilizan para títulos y subtítulos. Hay seis niveles de encabezados (`<h1>` a `<h6>`), siendo `<h1>` el más importante y `<h6>` el menos importante.
   ```html
   <h1>Este es un encabezado de nivel 1</h1>
   <h2>Este es un encabezado de nivel 2</h2>
   ```

2. **Párrafos**: Utiliza la etiqueta `<p>` para crear párrafos.
   ```html
   <p>Este es un párrafo de texto.</p>
   ```

3. **Listas**: 
   - **Listas desordenadas** (`<ul>`): Cada ítem en la lista se coloca dentro de una etiqueta `<li>`.
     ```html
     <ul>
         <li>Ítem 1</li>
         <li>Ítem 2</li>
         <li>Ítem 3</li>
     </ul>
     ```
   - **Listas ordenadas** (`<ol>`): Cada ítem se coloca dentro de una etiqueta `<li>`.
     ```html
     <ol>
         <li>Ítem 1</li>
         <li>Ítem 2</li>
         <li>Ítem 3</li>
     </ol>
     ```

4. **Imágenes**: Usa la etiqueta `<img>` y el atributo `src` para añadir imágenes.
   ```html
   <img src="url_de_la_imagen.jpg" alt="Descripción de la imagen">
   ```

5. **Enlaces**: Utiliza la etiqueta `<a>` para crear enlaces. El atributo `href` especifica la URL a la que apunta el enlace.
   ```html
   <a href="https://www.google.com">Ir a Google</a>
   ```

6. **Comentarios**: Los comentarios en HTML se insertan entre `<!--` y `-->`.
   ```html
   <!-- Este es un comentario -->
   ```

### Introducción a CSS

CSS (Cascading Style Sheets) se utiliza para controlar el diseño y la presentación de un documento HTML.

#### Añadir CSS a un Documento HTML

Hay tres maneras de añadir CSS a un documento HTML:

1. **CSS en línea**: Se aplica directamente a un elemento HTML utilizando el atributo `style`.
   ```html
   <p style="color: red;">Este es un párrafo con texto rojo.</p>
   ```

2. **CSS interno**: Se coloca dentro de una etiqueta `<style>` en la sección `<head>`.
   ```html
   <head>
       <style>
           body {
               background-color: lightblue;
           }
       </style>
   </head>
   ```

3. **CSS externo**: Se coloca en un archivo separado con extensión `.css` y se enlaza en el documento HTML.
   ```html
   <head>
       <link rel="stylesheet" href="styles.css">
   </head>
   ```

#### Selectores CSS

Los selectores CSS se utilizan para "seleccionar" el elemento HTML que quieres estilizar.

1. **Selector de elemento**: Aplica estilos a todos los elementos de un tipo.
   ```css
   p {
       color: blue;
   }
   ```

2. **Selector de clase**: Aplica estilos a elementos con una clase específica. Las clases se definen con un punto (`.`) antes del nombre de la clase.
   ```css
   .miClase {
       color: red;
   }
   ```

3. **Selector de ID**: Aplica estilos a un elemento con un ID específico. Los IDs se definen con un hash (`#`) antes del nombre del ID.
   ```css
   #miID {
       color: green;
   }
   ```

### Propiedades CSS Básicas

1. **Color de fondo**: Cambia el color de fondo de un elemento.
   ```css
   body {
       background-color: lightblue;
   }
   ```

2. **Color del texto**: Cambia el color del texto.
   ```css
   h1 {
       color: blue;
   }
   ```

3. **Bordes**: Aplica bordes a un elemento.
   ```css
   img {
       border: 2px solid black;
   }
   ```

4. **Fuente del texto**: Cambia la fuente del texto.
   ```css
   p {
       font-family: Arial, sans-serif;
   }
   ```

5. **Alineación del texto**: Alinea el texto al centro, a la izquierda o a la derecha.
   ```css
   p {
       text-align: center;
   }
   ```

6. **Margen**: Añade espacio alrededor de un elemento.
   ```css
   h1 {
       margin: 20px;
   }
   ```

7. **Relleno (padding)**: Añade espacio dentro de un elemento, entre el contenido y el borde.
   ```css
   ol li {
       padding: 10px;
   }
   ```

8. **Efectos al pasar el ratón (hover)**: Cambia el estilo de un elemento cuando el ratón pasa sobre él.
   ```css
   a:hover {
       color: red;
   }
   ```

9. **Ancho**: Define el ancho de un elemento.
   ```css
   img {
       width: 50%;
   }
   ```

### Formularios

Un formulario HTML permite a los usuarios enviar datos a un servidor. Los elementos básicos de un formulario incluyen campos de texto, botones de envío, etc.

#### Estructura de un Formulario

```html
<form action="url_a_donde_enviar_datos" method="post">
    <label for="nombre">Nombre:</label>
    <input type="text" id="nombre" name="nombre">
    
    <label for="password">Contraseña:</label>
    <input type="password" id="password" name="password">
    
    <input type="submit" value="Enviar">
</form>
```

### Tablas

Las tablas en HTML se utilizan para mostrar datos en un formato tabular.

#### Estructura de una Tabla

```html
<table>
    <tr>
        <th>Encabezado 1</th>
        <th>Encabezado 2</th>
        <th>Encabezado 3</th>
    </tr>
    <tr>
        <td>Dato 1</td>
        <td>Dato 2</td>
        <td>Dato 3</td>
    </tr>
    <tr>
        <td>Dato 4</td>
        <td>Dato 5</td>
        <td>Dato 6</td>
    </tr>
</table>
```

### Conclusión

Con estos conceptos básicos, deberías ser capaz de completar los primeros 30 ejercicios de HTML y CSS. 


---

## [Autor: Alejandro Di Stefano](https://github.com/Drako01)