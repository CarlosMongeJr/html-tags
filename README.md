# Etiquetas de HTML

La etiqueta de ***"comentario"*** se utiliza para insertar comentarios en el codigo fuente. Los comentarios no se muestran en el navegador. 
Se pueden usar comentarios para explicar el codigo, lo que puede ser especialmente util si se tiene mucho codigo.

```html
<!-- Este es un comentario -->
```

<br>

La declaración ***"DOCTYPE"*** no es una etiqueta HTML. Es una "información" para el navegador sobre qué tipo de documento esperar.

```html
<!DOCTYPE>
```

<br>

La etiqueta ***"a"*** define un hipervínculo, que se utiliza para enlazar de una página a otra.
El atributo más importante del elemento "a" es el atributo "href", que indica el destino del enlace.

```html
<a href="https://google.com"> Enlace a Google.com </a>
```

<br>

La etiqueta ***"abbr"*** define una abreviatura o un acrónimo, como "HTML", "CSS", "Dr."
Se usa el atributo global de "title" para mostrar la descripción de la abreviatura/acrónimo cuando pase el mouse sobre el elemento.

```htlm
El <abbr title="HyperText Markup Language">HTML</abbr> fue escrita por Tim Berners-Lee.
```

<br>

La etiqueta ***"address"*** define la información de contacto del autor/propietario de un documento o artículo.
La información de contacto puede ser una dirección de correo electrónico, URL, dirección física, número de teléfono, identificador de redes sociales, etc.
El texto en el elemento "address" generalmente se representa en cursiva.

```html
<address> Escrito por un Servidor </address>
```

<br>

La etiqueta ***"area"*** define un área dentro de un mapa de imagen (un mapa de imagen es una imagen con áreas en las que se puede hacer clic).
Los elementos "area" siempre están anidados dentro de una etiqueta "map".
***Nota:*** El atributo (usemap) en "img" está asociado con el atributo (name) del elemento "map" y crea una relación entre la imagen y el mapa.

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">

<map name="workmap">
  <area shape="rect" coords="34,44,270,350" alt="Computadora" href="computer.htm">
  <area shape="rect" coords="290,172,333,250" alt="Celular" href="phone.htm">
  <area shape="circle" coords="337,300,44" alt="Taza" href="coffee.htm">
</map>
```

<br>

