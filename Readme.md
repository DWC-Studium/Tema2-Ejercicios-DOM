<h1>Ejercicios Buscar</h1>
<h2>Ejercicio 1</h2>
<p>Mira esta página:</p>

        <html>
        <body>
          <div>Users:</div>
          <ul>
            <li>Juan</li>
            <li>Pedro</li>
          </ul>
        </body>
        </html>

<p>Para cada uno de los siguientes elementos, da al menos una manera de acceder a ellos:</p>
<ol>
    <li>El nodo DOM &lt;div&gt;</li>
    <li>El nodo DOM &lt;ul&gt;</li>
    <li>El segundo &lt;li&gt; (el de Pedro)</li>
</ol>

<h2>Ejercicio 2</h2>
<p>Escribe el código para pintar de rojo todas las celdas diagonales de una tabla.</p>
<p>Necesitarás seleccionar todos los td de table y pintarlos con el código:</p>

        // td debe referenciar a la celda
        td.style.backgroundColor = 'red';

<h2>Ejercicio 3</h2>
<p>Dada la siguiente página web:</p>

        <!DOCTYPE HTML>
        <html>
        <body>
          <form name="search">
            <label>Search the site:
              <input type="text" name="search">
            </label>
            <input type="submit" value="Search!">
          </form>

          <hr>

          <form name="search-person">
            Search the visitors:
            <table id="age-table">
              <tr>
                <td>Age:</td>
                <td id="age-list">
                  <label>
                    <input type="radio" name="age" value="young">less than 18</label>
                  <label>
                    <input type="radio" name="age" value="mature">18-50</label>
                  <label>
                    <input type="radio" name="age" value="senior">more than 50</label>
                </td>
              </tr>

              <tr>
                <td>Additionally:</td>
                <td>
                  <input type="text" name="info[0]">
                  <input type="text" name="info[1]">
                  <input type="text" name="info[2]">
                </td>
              </tr>

            </table>

            <input type="submit" value="Search!">
          </form>
        </body>
        </html>
<p>¿Cómo encontramos...?</p>
<ul>
    <li>la tabla con id="age-table".</li>
    <li>Todos los elementos label dentro de esa tabla (debe haber 3 de ellos).</li>
    <li>El primer td en esa tabla (con la palabra "Age").</li>
    <li>El form con name="search".</li>
    <li>El primer input en ese formulario.</li>
    <li>El último input en ese formulario.</li>
</ul>
<p>Abre la página en una ventana y usa las herramientas del navegador para ello.</p>

<h2>Ejercicio 7</h2>
<p>Poner en color naranja todos los enlaces externos alterando su propiedad style.</p>
<p>Un enlace es externo si:</p>
<ol>
    <li>Su href tiene :// en él.</li>
    <li>Pero no empieza con http://internal.com.</li>
</ol>
<p>Ejemplo:</p>

        <a name="list">the list</a>
        <ul>
          <li><a href="http://google.com">http://google.com</a></li>
          <li><a href="/tutorial">/tutorial.html</a></li>
          <li><a href="local/path">local/path</a></li>
          <li><a href="ftp://ftp.com/my.zip">ftp://ftp.com/my.zip</a></li>
          <li><a href="http://nodejs.org">http://nodejs.org</a></li>
          <li><a href="http://internal.com/test">http://internal.com/test</a></li>
        </ul>

        <script>
          // setting style for a single link
          let link = document.querySelector('a');
          link.style.color = 'orange';
        </script>

<h1>Ejercicios Modificar</h1>
<h2>Ejercicio 3</h2>
<p>Escribir una interfaz para crear una lista a partir de un la entrada del usuario.</p>
<p>Para cada item de la lista:</p>
<ol>
<p>Preguntar a un usuario sobre su contenido usando prompt.</p>
<p>Crear el li con ese contenido y añadirlo a ul.</p>
<p>Continuar hasta que el usuario cancela el input (presionando Esc o CANCELAR en el prompt).</p>
</ol>
<p>Todos los elementos deberían crearse dinámicamente.</p>
<p>Si un usuario escribe etiquetas HTML, deberían tratarse como texto.</p>
