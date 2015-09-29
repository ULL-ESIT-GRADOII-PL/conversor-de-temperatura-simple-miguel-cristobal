# ETSII ULL Grado de Informatica

## Práctica: Conversor en JavaScript de grados Celsius a Farenheit y viceversa

### Que aprendemos

* JavaScript básico
* Expresiones Regulares
* Uso de Emmet
* Uso de Mocha y Chai

### Diferencias con la versión en la rama `master`

* En la rama `html5pattern` el tag `<input>` se metió dentro de una form.

        <form id="formulario" onsubmit="calculate();">

* Además el `<input>` está controlado con el atributo `pattern` HTML5 de `<input>`:

        <input id="original"
               placeholder="32F"
               size="50"
               title = "Escribe un número seguido de una de las letras 'F' o 'C'"
               pattern="([-+]?\d+(?:\.\d*)?)\s*([fFcC])"
        />

* El fichero `pattern.html` tiene ejemplos de como usar el atributo `pattern`

          <form>
            <fieldset>
              <p><label>Caracteres alfanuméricos:</label><input type="text" pattern="[a-zA-Z0-9]+" /></p>
              <p><label>Letras:</label><input type="text" pattern="[a-zA-Z]+" /></p>
              <p><label>Números:</label><input type="text" pattern="[0-9]+" /></p>
              <p><label>Fecha (dd/mm/YYYYYY):</label><input type="text" pattern="(0[1-9]|[12][0-9]|3[01])[- /.](0[1-9]|1[012])[- /.](19|20)\d\d" /></p>
              <p><label>Email:</label><input type="text" pattern="[a-zA-Z0-9.+_-]+@[a-zA-Z0-9.-]+\.[a-zA-Z0-9.-]+" /></p>
              <input id="final" type="submit" value="Aceptar" />
            </fieldset>
          </form>

* En esta rama en `temperature.js` se usa `alert` para enviar los mensajes en vez de insertarlos en la página con el método `innerHTML`.
