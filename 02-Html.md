# HTML Referencia rapida
## Tags HTML Más Usados

| Tag          | Descripción                                                                            | Ejemplo                                      |
|--------------|----------------------------------------------------------------------------------------|----------------------------------------------|
| `<html>`     | Documento HTML. Es el contenedor raíz de todos los demás elementos.                    | `<html>...</html>`                           |
| `<head>`     | Contiene metadatos e información como el título y enlaces a estilos o scripts.         | `<head>...</head>`                           |
| `<title>`    | Título del documento que se muestra en la pestaña del navegador.                       | `<title>Mi pagina</title>`                   |
| `<body>`     | Contenido visible de la página web.                                                    | `<body>...</body>`                           |
| `<h1> - <h6>`| Encabezados, siendo `<h1>` el más importante y `<h6>` el menos importante.             | `<h1>Titulo</h1>`                            |
| `<p>`        | Párrafo de texto.                                                                      | `<p>This is a paragraph.</p>`                |
| `<a>`        | Hipervínculo para enlaces a otras páginas o partes de la misma página.                 | `<a href="url">Link</a>`                     |
| `<img>`      | Inserta imagen en la página.                                                           | `<img src="./image.jpg" alt="Description">`  |
| `<div>`      | Contenedor genérico. Útil para agrupar contenido y aplicar estilos.                    | `<div>...</div>`                             |
| `<span>`     | Contenedor en línea, usada principalmente para aplicar estilos a partes de un texto.   | `<span>Text</span>`                          |
| `<ul>`       | Lista desordenada (bullet points).                                                     | `<ul><li>Item</li></ul>`                     |
| `<ol>`       | Lista ordenada (numerada).                                                             | `<ol><li>Item</li></ol>`                     |
| `<li>`       | Define un ítem dentro de una lista (`<ul>` o `<ol>`).                                  | `<li>List Item</li>`                         |
| `<form>`     | Formulario para la entrada de datos del usuario.                                       | `<form>...</form>`                           |
| `<input>`    | Entrada interactivo dentro de un formulario (campo de texto, checkbox, etc.).          | `<input type="text">`                        |
| `<button>`   | Botón interactivo.                                                                     | `<button>Click Me</button>`                  |
| `<table>`    | Tabla para organizar datos en filas y columnas.                                        | `<table>...</table>`                         |
| `<th>`       | Define una celda de encabezado en una tabla.                                           | `<th>Header</th>`                            |
| `<td>`       | Define una celda de datos en una tabla.                                                | `<td>Data</td>`                              |
| `<tr>`       | Define una fila en una tabla.                                                          | `<tr>...</tr>`                               |
| `<header>`   | Define un encabezado de la página o de una sección.                                    | `<header>...</header>`                       |
| `<footer>`   | Define un pie de página o de sección.                                                  | `<footer>...</footer>`                       |
| `<nav>`      | Define un conjunto de enlaces de navegación.                                           | `<nav>...</nav>`                             |
| `<section>`  | Define una sección del documento, agrupando contenido relacionado.                     | `<section>...</section>`                     |
| `<article>`  | Define contenido independiente y autocontenido.                                        | `<article>...</article>`                     |
| `<aside>`    | Define contenido secundario relacionado, como una barra lateral.                       | `<aside>...</aside>`                         |

---
## Extructura basica de HTML
```html
<!DOCTYPE html>
<html lang="es">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Título de la Página</title>
    <link rel="stylesheet" href="styles.css"> <!-- Enlace a tu archivo CSS -->
  </head>
  <body>
    <header>
      <h1>Encabezado Principal</h1>
      <nav>
        <ul>
          <li><a href="#">Inicio</a></li>
          <li><a href="#">Acerca</a></li>
          <li><a href="#">Contacto</a></li>
        </ul>
      </nav>
    </header>
  
    <main>
      <section>
        <h2>Sección 1</h2>
        <p>Este es un párrafo dentro de la sección.</p>
      </section>
      
      <section>
        <h2>Sección con una Tabla</h2>
        <table>
          <thead>
            <tr>
              <th>Nombre</th>
              <th>Edad</th>
              <th>Ciudad</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Juan Pérez</td>
              <td>30</td>
              <td>Madrid</td>
            </tr>
            <tr>
              <td>María López</td>
              <td>25</td>
              <td>Barcelona</td>
            </tr>
            <tr>
              <td>Carlos Sánchez</td>
              <td>28</td>
              <td>Sevilla</td>
            </tr>
          </tbody>
        </table>
      </section>
    </main>
  
    <footer>
      <p>2024 Todos los derechos reservados.</p>
    </footer>
  
  </body>
</html>
```
---
## Extructura de Tag select
En HTML, el elemento `<select>` se utiliza para crear un menú desplegable donde el usuario puede seleccionar una opción o varias opciones de una lista.
### Sintaxis basica
```html
<select name="nombre">
  <option value="valor1">Opción 1</option>
  <option value="valor2">Opción 2</option>
  <option value="valor3">Opción 3</option>
</select>
```
### Atributos importantes
- `name`: Nombre que se enviará en el formulario.
- `multiple`: Permite seleccionar más de una opción (si se especifica).
- `disabled`: Desactiva el menú desplegable.
- `size`: Define cuántas opciones se muestran al mismo tiempo (sin desplegar).

### Ejemplos con atributos
- Seleccion desplegable
```html
<form action="/submit" method="post">
  <label for="frutas">Selecciona una fruta:</label>
  <select name="frutas" id="frutas">
    <option value="manzana">Manzana</option>
    <option value="naranja">Naranja</option>
    <option value="banana">Banana</option>
  </select>
  <button type="submit">Enviar</button>
</form>
```
- Seleccion multiple
```html
<form action="/submit" method="post">
  <label for="lenguajes">Selecciona tus lenguajes favoritos:</label>
  <select name="lenguajes" id="lenguajes" multiple size="3">
    <option value="html">HTML</option>
    <option value="css">CSS</option>
    <option value="javascript">JavaScript</option>
  </select>
  <button type="submit">Enviar</button>
</form>
```
