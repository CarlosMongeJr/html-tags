# Etiquetas de HTML

### ***&lt;!--...--&gt;***
La etiqueta de ***"&lt;!-- --&gt;"*** se utiliza para insertar comentarios en el codigo fuente. Los comentarios no se muestran en el navegador. 
Se pueden usar comentarios para explicar el codigo, lo que puede ser especialmente util si se tiene mucho codigo.

```html
<!-- Este es un comentario -->
```

<br>

### ***&lt;!DOCTYPE&gt;***
La declaración ***"DOCTYPE"*** no es una etiqueta HTML. Es una "información" para el navegador sobre qué tipo de documento esperar.

```html
<!DOCTYPE html>
```

<br>

### ***&lt;a&gt;***
La etiqueta ***"a"*** define un hipervínculo, que se utiliza para enlazar de una página a otra.
El atributo más importante del elemento "a" es el atributo "href", que indica el destino del enlace.

```html
<a href="https://google.com"> Enlace a Google.com </a>
```

<br>

### ***&lt;abbr&gt;***
La etiqueta ***"abbr"*** define una abreviatura o un acrónimo, como "HTML", "CSS", "Dr."
Se usa el atributo global de "title" para mostrar la descripción de la abreviatura/acrónimo cuando pase el mouse sobre el elemento.

```htlm
El <abbr title="HyperText Markup Language">HTML</abbr> fue escrita por Tim Berners-Lee.
```

<br>

### ***&lt;address&gt;***
La etiqueta ***"address"*** define la información de contacto del autor/propietario de un documento o artículo.
La información de contacto puede ser una dirección de correo electrónico, URL, dirección física, número de teléfono, identificador de redes sociales, etc.
El texto en el elemento "address" generalmente se representa en cursiva.

```html
<address> Escrito por <a href="mailto:webmaster@example.com">Jon Doe</a>.</address>
```

<br>

### ***&lt;area&gt;***
La etiqueta ***"area"*** define un área dentro de un mapa de imagen (un mapa de imagen es una imagen con áreas en las que se puede hacer clic).
Los elementos "area" siempre están anidados dentro de una etiqueta "map".

***Nota:*** El atributo (usemap) en "img" está asociado con el atributo (name) en "map" y crea una relación entre la imagen y el mapa.

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">
<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computadora" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Celular" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Taza" href="coffee.htm">
</map>
```

<br>

### ***&lt;article&gt;***
La etiqueta ***"article"*** especifica contenido independiente.
Un article debe tener sentido por sí mismo y debe ser posible distribuirlo independientemente del resto del sitio.
Fuentes potenciales para el elemento article:
* Publicación en el foro
* Entrada en el blog
* Noticia

```html
<article>
  <h1>Navegadores más populares</h1>
  <h2>Google Chrome</h2>
  <p>Google Chrome es un navegador web desarrollado por Google y el más popular del mundo!</p>
</article>
```

<br>

### ***&lt;aside&gt;***
La etiqueta ***"aside"*** define algún contenido además del contenido en el que se coloca.
El contenido aparte debe estar indirectamente relacionado con el contenido circundante.

***Nota:*** El contenido "aside" a menudo se coloca como una barra lateral en un documento.

```html
<aside>
  <p>El centro Epcot es un parque temático en Walt Disney World Resort.</p>
</aside>
```

<br>

### ***&lt;audio&gt;***
La etiqueta ***"audio"*** se usa para incrustar contenido de sonido en un documento, como música u otras transmisiones de audio.
La etiqueta 'audio' contiene una o más etiquetas "source" con diferentes fuentes de audio. El navegador elegirá la primera fuente que admita.
El texto entre las etiquetas 'audio' solo se mostrará en navegadores que no admitan el elemento 'audio'.

Hay tres formatos de audio admitidos en HTML: ( MP3, WAV y OGG. )

```html
<audio>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
  Su navegador no es compatible con la etiqueta de audio.
</audio>
```

<br>

### ***&lt;b&gt;***
La etiqueta ***"b"*** especifica texto en negrita sin ninguna importancia adicional.

***Nota:*** De acuerdo con la especificación de HTML5, la etiqueta "b" debe usarse como ***ULTIMO*** recurso cuando ninguna otra etiqueta sea más apropiada. La especificación establece que el texto enfatizado debe indicarse con la etiqueta "em", el texto importante con la etiqueta "strong" y el texto marcado/resaltado con la etiqueta "mark".

```html
<p> Este es texto normal <b>y este es texto en negrita</b> </p>
```

<br>

### ***&lt;base&gt;***
La etiqueta ***"base"*** especifica la URL base y/o el destino de todas las URL relativas en un documento.
La etiqueta "base" debe tener presente un atributo href o target, o ambos.
Solo puede haber un único elemento "base" en un documento, y debe estar dentro del elemento "head".

 ***Nota:*** Tenga en cuenta que solo hemos especificado una dirección relativa para la imagen. Dado que hemos especificado una URL base en la sección principal, el navegador buscará la imagen en "https://www.w3schools.com/images/stickman.gif".

```html
<head>
  <base href="https://www.w3schools.com/" target="_blank">
</head>
<body>
  <img src="images/stickman.gif" width="24" height="39" alt="Stickman">
</body>
```

<br>

### ***&lt;bdi&gt;***
BDI significa aislamiento bidireccional.

La etiqueta ***"bdi"*** le dice al algoritmo bidireccional del navegador que trate el texto que contiene de forma aislada del texto que lo rodea. 
Es particularmente útil cuando un sitio web inserta texto de forma dinámica que podría estar formateada en una dirección diferente de otro texto fuera de ella y no conoce la direccionalidad del texto que se inserta.

```html
<ul>
 <li>Usuario 1<bdi> hrefs </bdi></li>
 <li>Usuario 2<bdi> jdoe </bdi></li>
 <li>Usuario 3<bdi> إيان </bdi></li>
</ul>
```

<br>

### ***&lt;bdo&gt;***
BDO significa anulación bidireccional.

La etiqueta ***"bdo"*** se utiliza para anular la dirección del texto actual y tiene 2 valores "rtl" (right to left) y "ltr" (left to right).

```html
<bdo dir="rtl">
  Este texto irá de derecha a izquierda.
</bdo>
```

<br>

### ***&lt;blockquote&gt;***
La etiqueta ***"blockquote"*** especifica una sección que se cita de otra fuente.
Los navegadores suelen endentar los elementos "blockquote".

***Nota:*** El atributo (cite) especifica la fuente de la cita.

```html
<blockquote cite="http://www.worldwildlife.org/who/index.html">
  WWF, la organización de conservación líder en el mundo, cuenta con cerca de 5 millones de miembros en todo el mundo.
</blockquote>
```

<br>

### ***&lt;body&gt;***
La etiqueta ***"body"*** define el cuerpo del documento.
El elemento "body" contiene todo el contenido de un documento HTML, como encabezados, párrafos, imágenes, hipervínculos, tablas, listas, etc.

***Nota:*** Solo puede haber un elemento "body" en un documento HTML.

```html
<body>
  <h1>Este es un encabezado</h1>
  <p>Esto es un párrafo.</p>
  <img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
  <a href="https://www.w3schools.com">¡Visite W3Schools.com!</a>
</body>
```

<br>

### ***&lt;br&gt;***
La etiqueta ***"br"*** inserta un solo salto de línea; es útil para escribir direcciones o poemas.
La etiqueta "br" es una etiqueta vacía, lo que significa que no tiene una etiqueta final.

***Nota:*** Utilice la etiqueta "br" para introducir saltos de línea, no para añadir espacios entre párrafos.

```html
<p>
  Tan bellos es el Sol<br>
  tan bella es la Luna<br>
  a alguien como Tu<br>
  no la cambio por ninguna<br>
</p>
```

<br>

### ***&lt;button&gt;***
La etiqueta ***"button"*** define un botón en el que se puede hacer clic.

***Nota:*** Si sus botones no son para enviar datos de formulario a un servidor, asegúrese de establecer su atributo de (type) en "button". 
De lo contrario, intentarán enviar los datos del formulario y cargar la respuesta (inexistente), posiblemente destruyendo el estado actual del documento.

```html
<button type="button">¡Haz click</button>
```
  
<br>

### ***&lt;canvas&gt;***
La etiqueta ***"canvas"*** se usa para dibujar gráficos, sobre la marcha, a través de secuencias de comandos (generalmente JavaScript).
La etiqueta "canvas" es transparente y es solo un contenedor para gráficos, (se debe usar un "script" para dibujar los gráficos).

***Nota:*** Cualquier texto dentro del elemento "canvas" se mostrará en navegadores con JavaScript deshabilitado y en navegadores que no admitan "canvas".

```html
<canvas id="myCanvas">
    Su navegador no admite la etiqueta de canvas.
</canvas>
    
<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");

  ctx.fillStyle = "red";
  ctx.fillRect(20, 20, 75, 50);
  //Turn transparency on
  // ctx.globalAlpha = 0.2;
  ctx.fillStyle = "blue";
  ctx.fillRect(50, 50, 75, 50);

  ctx.fillStyle = "green";
  ctx.fillRect(80, 80, 75, 50);
</script>
```

<br>

### ***&lt;caption&gt;***
La etiqueta ***"caption"*** define un título de tabla.
La etiqueta "caption" debe insertarse inmediatamente después de la etiqueta "table".

***Nota:*** Por defecto, el título de una tabla se alineará al centro sobre una tabla. Sin embargo, las propiedades CSS text-align y caption-side se pueden usar para alinear y colocar el título.

```html
<tabla>
   <caption>Ahorros mensuales</caption>
   <tr>
     <th>Mes</th>
     <th>Ahorros</th>
   </tr>
   <tr>
     <td>enero</td>
     <td>$100</td>
   </tr>
   <tr>
     <td>febrero</td>
     <td>$50</td>
   </tr>
</tabla>
```

<br>

### ***&lt;cite&gt;***
La etiqueta ***"cite"*** define el título de una obra creativa (por ejemplo, un libro, un poema, una canción, una película, una pintura, una escultura, etc.).
El nombre de una persona no es el título de una obra.

***Nota:*** El texto en el elemento "cite" generalmente se presenta en itálica.

```html
<p>
  <cite>El grito</cite> de Edvard Munch. Pintado en 1893.
</p>
```

<br>

### ***&lt;code&gt;***
La etiqueta ***"code"*** se usa para definir una pieza de código de computadora. El contenido del interior se muestra en la fuente (monospace) predeterminada del navegador.

***Nota:*** Se utiliza principalmente para mostrar el fragmento de código en el navegador web.

```html
<p>La propiedad CSS <code>background-color</code> define el color de fondo de un elemento.</p>
```

<br>

### ***&lt;col&gt;***
La etiqueta ***"col"*** especifica las propiedades de columna para cada columna dentro de un elemento "colgroup".
La etiqueta "col" es útil para aplicar estilos a columnas enteras, en lugar de repetir los estilos para cada celda, para cada fila.

```html
<table>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
</table>
```

<br>

### ***&lt;colgroup&gt;***
La etiqueta ***"colgroup"*** especifica un grupo de una o más columnas en una tabla para formatear.

***Nota:*** La etiqueta "colgroup" debe ser hijo de un elemento "table" y antes de cualquier elemento "thead", "tbody", "tfoot" y "tr".

<br>
  
```html
 <table>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <tr>
    <th>Titulo</th>
    <th>Precio</th>
  </tr>
  <tr>
    <td>Mi libro HTML</td>
    <td>$53</td>
  </tr>
</table> 
```

<br>

### ***&lt;data&gt;***
La etiqueta ***"data"*** se usa para agregar una traducción legible por máquina de un contenido determinado.
Este elemento proporciona un valor legible por máquina para los procesadores de datos y un valor legible por humanos para la representación en un navegador.

***Nota:*** si el contenido está relacionado con la hora o la fecha, utilice el elemento (time) en su lugar.

```html
<ul>
  <li><data value="21053">Tomate cherry</data></li>
  <li><data value="21054">Tomate de ternera</data></li>
  <li><data value="21055">Tomate de merienda</data></li>
</ul>
```

<br>

### ***&lt;datalist&gt;***
La etiqueta ***"datalist"*** especifica una lista de opciones predefinidas para un elemento "input".
La etiqueta "datalist" se utiliza para proporcionar una función de "autocompletar" para los elementos "input".

***Nota:*** El atributo (id) del elemento "datalist" debe ser igual al atributo (list) del elemento "input" ***(esto los une).***

```html
<label for="browser">Elija su navegador de la lista:</label>
<input list="browsers" name="browser" id="browser">

<datalist id="browsers">
  <option value="Edge">
  <option value="Firefox">
  <option value="Chrome">
  <option value="Opera">
  <option value="Safari">
</datalist>
```

<br>

### ***&lt;dd&gt;***
La etiqueta ***"dd"*** se utiliza para describir un término/nombre en una lista de descripción.
La etiqueta "dd" se usa junto con "dl" (define una lista de descripciones) y "dt" (define términos/nombres).

Dentro de una etiqueta "dd" puedes poner párrafos, saltos de línea, imágenes, enlaces, listas, etc.

```html
<dl>
   <dt>Café</dt>
   <dd>Bebida negra caliente</dd>
   <dt>Leche</dt>
   <dd>Bebida blanca fría</dd>
</dl>
```

<br>

### ***&lt;del&gt;***
La etiqueta ***"del"*** define el texto que se ha eliminado de un documento. Los navegadores generalmente marcarán una línea a través del texto eliminado.

```html
<p>¡Mi color favorito es <del>verde</del> azul!</p>
```

<br>

### ***&lt;details&gt;***
La etiqueta ***"details"*** especifica detalles adicionales y se usa a menudo para crear un widget interactivo que el usuario puede abrir y cerrar. 
De forma predeterminada, el widget está cerrado. Cuando está abierto, se expande y muestra el contenido que contiene.

***Nota:*** la etiqueta "summary" se utiliza junto con "details" para especificar un encabezado visible para los detalles.

```html
<details>
  <summary>Cuanto cuesta la membresia?</summary>
  <p>La memebresia es gratis el primer año.</p>
</details>
```

<br>

### ***&lt;dfn&gt;***
La etiqueta ***"dfn"*** representa el "elemento de definición" y especifica un término que se definirá dentro del contenido.
El padre más cercano de la etiqueta "dfn" también debe contener la definición/explicación del término.

```html
<p> <dfn>HTML</dfn> es el lenguaje de marcado estándar para crear páginas web. </p>
```

<br>

### ***&lt;dialog&gt;***
La etiqueta ***"dialog"*** define un cuadro de diálogo o una subventana.
El elemento "dialog" facilita la creación de cuadros de diálogo emergentes y modales en una página web.

```html
<dialog open>Esta es una ventana de diálogo abierta</dialog>
```

<br>

### ***&lt;div&gt;***
La etiqueta ***"div"*** define una división o una sección en un documento HTML.
La etiqueta "div" se utiliza como contenedor de elementos HTML, que luego se diseñan con CSS o se manipulan con JavaScript usando el atributo (class o id).
¡Se puede poner cualquier tipo de contenido dentro de la etiqueta "div"!

***Nota:*** De forma predeterminada, los navegadores siempre colocan un salto de línea antes y después del elemento "div".

```html
<div class="miDiv">
  <h2>Este es un encabezado en un elemento div</h2>
  <p>Este es un parrafo en un elemento div</p>
</div>
```

<br>

### ***&lt;dl&gt;***
La etiqueta ***"dl"*** define una lista de descripción.
La etiqueta "dl" se usa junto con "dt" (define términos/nombres) y "dd" (describe cada término/nombre).
  
```html
<dl>
   <dt>Café</dt>
   <dd>Bebida negra caliente</dd>
   <dt>Leche</dt>
   <dd>Bebida blanca fría</dd>
</dl>
```

<br>

### ***&lt;dt&gt;***
La etiqueta ***"dt"*** define un término/nombre en una lista de descripción.
La etiqueta "dt" se usa junto con "dl" (define una lista de descripción) y "dd" (describe cada término/nombre).

```html
<dl>
   <dt>Café</dt>
   <dd>Bebida negra caliente</dd>
   <dt>Leche</dt>
   <dd>Bebida blanca fría</dd>
</dl>
```

<br>

### ***&lt;em&gt;***
La etiqueta ***"em"*** se utiliza para definir texto enfatizado. El contenido interior normalmente se muestra en cursiva.
Un lector de pantalla pronunciará las palabras en "em" con énfasis, usando acento verbal.

```html
<p>¡Tú <em>tienes</em> que darte prisa!</p>
```

<br>

### ***&lt;embed&gt;***
La etiqueta ***"embed"*** define un contenedor para un recurso externo, como una página web, una imagen, un reproductor multimedia o una aplicación complementaria.

***Nota:*** Para mostrar una imagen, es mejor usar la etiqueta "img". Para mostrar HTML, la etiqueta "iframe" y para mostrar video o audio, es mejor usar las etiquetas "video" y "audio".
  
```html
<embed type="image/jpg" src="pic_trulli.jpg" width="300" height="200">
<embed type="text/html" src="snippet.html" width="500" height="200">
<embed type="video/webm" src="video.mp4" width="400" height="300">
```

<br>

### ***&lt;fieldset&gt;***
La etiqueta ***"fieldset"*** se usa para agrupar elementos relacionados en un formulario.
La etiqueta "fieldset" dibuja un cuadro alrededor de los elementos relacionados.

```html
<form>
 <fieldset>
  <legend>Personalidad:</legend>
  <label for="fname">Nombre:</label>
  <input type="text" id="fname" name="fname"><br><br>
  <label for="lname">Apellido:</label>
  <input type="text" id="lname" name="lname"><br><br>
  <label for="email">Correo:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="Submit">
 </fieldset>
</form>
```

<br>

### ***&lt;figcaption&gt;***
La etiqueta ***"figcaption"*** define un título para un elemento "figure".
El elemento "figcaption" se puede colocar como el primer o último hijo del elemento "figure".

```html
<figure>
  <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>
```

<br>

### ***&lt;figure&gt;***
La etiqueta ***"figure"*** especifica contenido independiente, como ilustraciones, diagramas, fotos, listas de códigos, etc.
Si bien el contenido del elemento "figure" está relacionado con el flujo principal, su posición es independiente del flujo principal y, si se elimina, no debería afectar el flujo del documento.

```html
<figure>
  <img src="pic_trulli.jpg" alt="Trulli" style="width:100%">
  <figcaption>Fig.1 - Trulli, Puglia, Italy.</figcaption>
</figure>
```

<br>

### ***&lt;footer&gt;***
La etiqueta ***"footer"*** define un pie de página para un documento o sección.

Un elemento "footer" normalmente contiene:

* información de autoría
* informacion registrada
* Información del contacto
* mapa del sitio
* volver a los enlaces superiores
* documentos relacionados
* Puede tener varios elementos <footer> en un documento.

***Nota:*** La información de contacto dentro de un elemento "footer" debe ir dentro de una etiqueta "address".
  
```html
<footer>
 <p>Autor: Hege Refsnes</p>
 <p><a href="mailto:hege@example.com">hege@example.com</a></p>
</footer>
  
<address>
  Written by <a href="mailto:webmaster@example.com">Jon Doe</a>.<br>
  Visit us at:<br>
  Example.com<br>
  Box 564, Disneyland<br>
  USA
</address>
```

<br>

### ***&lt;form&gt;***
### ***&lt;h1&gt;...to...&lt;h6&gt;***
### ***&lt;head&gt;***
