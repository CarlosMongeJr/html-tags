# Etiquetas de HTML

### ***&lt;!--...--&gt;***
La etiqueta de ***"comentario"*** se utiliza para insertar comentarios en el codigo fuente. Los comentarios no se muestran en el navegador. 
Se pueden usar comentarios para explicar el codigo, lo que puede ser especialmente util si se tiene mucho codigo.

```html
<!-- Este es un comentario -->
```

<br>

### ***&lt;!DOCTYPE&gt;***
La declaración ***"DOCTYPE"*** no es una etiqueta HTML. Es una "información" para el navegador sobre qué tipo de documento esperar.

```html
<!DOCTYPE>
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
Fuentes potenciales para el elemento article: (publicacion en el foro, entrada de blog, noticias)
* Publicación en el foro
* Entrada en el blog
* Noticia

```html
<article>
  <h1>Navegadores más populares</h1>
  <h2>Google Chrome</h2>
  <p>Google Chrome es un navegador web desarrollado por Google, lanzado en 2008. ¡Chrome es el navegador web más popular del mundo en la actualidad!</p>
</article>
```

<br>

### ***&lt;aside&gt;***
La etiqueta ***"aside"*** define algún contenido además del contenido en el que se coloca.
El contenido aparte debe estar indirectamente relacionado con el contenido circundante.
***Nota:*** El contenido "aside" a menudo se coloca como una barra lateral en un documento.

```html
<aside>
  <p>El centro Epcot es un parque temático en Walt Disney World Resort que cuenta con emocionantes atracciones y eventos especiales de temporada.</p>
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
