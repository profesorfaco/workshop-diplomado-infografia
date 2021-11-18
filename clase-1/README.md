# HTML y CSS

### Clase 1 → 18-11-2021

- - - - - - - 

## Presentación
 
**HTML (HyperText Markup Language) es un lenguaje estándar que describe la estructura de cada página web**. 

HTML5 es la versión más reciente de este lenguaje. Lo más básico del HTML es el elemento. 

Cada elemento de HTML se escribe entre etiquetas: `<etiqueta>contenido</etiqueta>`; habiendo excepciones que no son más que una etiqueta, tales como la imagen (`<img>`), el quiebre de línea (`<br>`), la línea horizontal (`<hr>`) o el metadato (`<meta>`). 

Las etiquetas utilizan "[palabras reservadas](http://html5doctor.com/element-index/)" entre paréntesis angulares de apertura (`<`) y cierre (`>`).

En la primera o única etiqueta que conforma el elemento, antes que se cierre el paréntesis angular (`>`), se pueden agregar atributos que contienen información  acerca del elemento. 

En algunos casos el atributo aporta información indispensable, como en la definción del recurso (`scr`) que se despliega como imagen (`img`):

```
<img src="foto.jpg">
```

En otros casos el atributo aporta información complementaria, como en un párrafo (`p`) con un atributo de clase (`class`) especial:

```
<p class="especial">Este es un párrafo especial</p>
```

Los navegadores web ofrecen la opción de "ver el código fuente de la página": aprovechemos tal opción para darle un vistazo al HTML de la primera infografía digital de El Mercurio: 

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/

Podemos ver aquellas partes que conforman tal HTML, gracias a las instrucciones en [este documento](http://infografias.elmercurio.com/20160722-VCT-basuraespacial/js/infografia.js):

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/header/header.html

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_01/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_02/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_03/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/gif/index.html

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_04/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/video/index.html

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_12/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/video2/index.html

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_06/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_07/
 
 - http://infografias.elmercurio.com/20160722-VCT-basuraespacial/gif2/index.html
 
- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_08/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_09/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_10/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_preinfo/

- http://infografias.elmercurio.com/20160722-VCT-basuraespacial/infografia/modulo_info/

- http://infografias.elmercurio.com/footer/footer.html

**Y podemos saltar al otro lado del mundo, para echarle un vistazo al código fuente de un par de páginas del South China Morning Post:**

- https://multimedia.scmp.com/infographics/news/hong-kong/article/3022630/hong-kong-airport-protest/

- https://multimedia.scmp.com/culture/article/ufo/

Como pudieron notar, en todas estas páginas se usan elementos `<etiqueta>contenido</etiqueta>` que no hacen más que describirse según un estándar amplio, pero limitado, de "[palabras reservadas](http://html5doctor.com/element-index/)". 

Existen muchos recursos en línea que ayudan a familiarizarse con estas `<etiquetas></etiquetas>`. Pueden buscar estos recursos como *cheat sheets*; un ejemplo: https://html.com/wp-content/uploads/html-cheat-sheet.pdf

- - - - - - - -- 

Ahora volvamos al principio, a lo más básico, y observemos cómo los elementos se describen estructurando un documento HTML:

```
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>¡Hola Mundo!</title>
  </head>
  <body>
    <h1>¡Hola Mundo!</h1>
  </body>
</html>
```

En lo recién observado, tenemos:

- Un anuncio `<!doctype html>` que nos indica que las líneas que siguen son las de un documento HTML en versión 5; así como una banderita en un sandwich puede anunciar la cadena de comida rápida donde se preparó.

- Un elemento `<html lang="es"></html>` que contiene a todo el documento HTML, que será escrito en español; este sería el pan del sandwich.

- Un elemento `<head></head>` que contiene indicaciones que describen y complementan lo que se mostrará en la ventana del navegador

- Un elemento `<body></body>` que contiene todo lo que se podría mostrar en la ventana del navegador.

- - - - - - - 

Pero el documento HTML necesita una forma de verse distinta de la definida para [el intercambio de trabajo científico](https://www.ted.com/speakers/tim_berners_lee?language=es) en la Organización Europea para la Investigación Nuclear, a fines de 1980 y comienzo de 1990 (fondo blanco, letras negras, tipografía con serifa en tamaños predefinidos y vínculos subryados en azul cuando aún no han sido visitados). Para ello el HTML se complementa con CSS.

**CSS (Cascading Style Sheets) es un lenguaje estándar que describe la presentación de las páginas web (cómo se muestra lo que contiene la página).**

CSS3 es la versión más reciente de este lenguaje. 

Lo más básico del CSS es la regla. Cada regla se inicia con un selector, seguido de paréntesis de llave `{…}`. Tal paréntesis contiene una o varias declaraciones. Cada declaración se compone del par `propiedad: valor`. Cuando son varias declaraciones, corresponde separar una de otra mediante punto y coma: 

```
selector{ 
 propiedad: valor;
 propiedad: valor;
}
```

El selector de cada regla CSS indica dónde y/o cuándo ésta debe afectar al HTML. Por ejemplo: 

```
a{
 color:red;
}

a[href$=".pdf"]{
 color:purple;
}

a:hover{
 color:pink;
}
```

En el ejemplo, tenemos:

- una primera regla afecta a todo vínculo (`a` de anchor), asignándole un color rojo. 

- una segunda regla afecta al vínculo si es que su referencia de hipertexto termina en .pdf (`href` de hipertext reference), asignándole un color púrpura.

- una tercera regla afecta a todo vínculo cuando el mouse pasa por encima, asignándole un color rosa en ese momento. 

**Ahora, para que el CSS afecte al documento HTML correspondiente, puede incrustarse, importarse o vincularse en la cabeza del mismo documento**:

Cuando se inscrusta, la cabeza del HTML queda así:

```
<head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 <style>
  a{
   color:red;
  }
  a[href$=".pdf"]{
   color:purple;
  }
  a:hover{
   color:pink;
  }
 </style>
 <title>¡Hola Mundo!</title>
</head>
```

Cuando se importa:

```
<head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 <style>
  @import url('estilo.css');
 </style>
 <title>¡Hola Mundo!</title>
</head>
```

Y cuando se vincula:

```
<head>
 <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 <link href="estilo.css" rel="stylesheet">
 <title>¡Hola Mundo!</title>
</head>
```

Para que no quede sin mencionarse, también se puede incluir CSS a nivel de atributos del HTML, pero esa es una forma poco eficiente porque afecta a un único elemento, el que lo contiene, y por lo mismo no utiliza selector ni paréntesis de llave, sólo usa el o los pares `propiedad: valor`.  

```
<a href="https://github.com/profesorfaco/infografia" style="color:red">este es un vínculo</a>
```

- - - - - - - 

## Exploración

**Existen marcos de trabajo de código abierto que nos pueden ayudar a avanzar más rápido desde relaciones predefinidas de HTML y CSS**. Por su popularidad, corresponde mencionar a:

- [Bootstrap](https://getbootstrap.com/): *The world’s most popular front-end open source toolkit, featuring Sass variables and mixins, responsive grid system, extensive prebuilt components, and powerful JavaScript plugins.*

- [Foundations](https://get.foundation/): *The most advanced responsive front-end framework in the world* 

- [Semantic UI](https://semantic-ui.com/): *A development framework that helps create beautiful, responsive layouts using human-friendly HTML*

Nos quedaremos con el primero de los mencionados, [Bootstrap](https://getbootstrap.com/). 

En los [Docs](https://getbootstrap.com/docs/5.1/getting-started/introduction/) de [Bootstrap](https://getbootstrap.com/) podemos ver cómo las relaciones predefinidas de HTML y CSS nos permiten crear:

- [Botones](https://getbootstrap.com/docs/5.0/components/buttons/)

- [Pase de diapositivas tipo carrusel](https://getbootstrap.com/docs/5.0/components/carousel/)

- [Notificaciones emergentes](https://getbootstrap.com/docs/5.0/components/toasts/)

- Y un largo etc.

Para sacarle buen provecho a [Bootstrap](https://getbootstrap.com/), lo primero es relacionarse con la lógica de las 12 columnas (`col`) en las que se puede dividir una fila (`row`) que se va ajustando dentro de un contenedor (`container`), porque esta es la lógica con la que [Bootstrap](https://getbootstrap.com/) se adapta a distintos tamaños de pantalla.

Digamos que en este contenedor (`container`) quiero dividir la fila (`row`) en dos partes del mismo ancho, para que una se muestre al lado de la otra. Para lograrlo debo tomar 6 y 6 columnas (`col`). Dentro del cuerpo del documento HTML, esto se vería así:

```
<div class="container">
 <div class="row">
  <div class="col-6">Primera división</div>
  <div class="col-6">Segunda división</div>
 </div>
</div>
```

Ahora, quiero hacer la misma división pero sólo desde una pantalla mediana ([mayor a 768px de ancho](https://getbootstrap.com/docs/5.0/layout/breakpoints/#available-breakpoints)). En las pantallas que tengan un ancho menor, ambas divisiones ocuparán todo el ancho, poniéndose la segunda debajo de la primera:

```
<div class="container">
 <div class="row">
  <div class="col-md-6">Primera división</div>
  <div class="col-md-6">Segunda división</div>
 </div>
</div>
```

Cambiemos de ejemplo, considerando que Robert Bringhurst (2008) escribe:

> La cantidad que se considera satisfactoria como longitud de línea para una página de una sola columna compuesta en una fuente con remates va entre 45 u 75 caracteres. La línea de 66 caracteres (contando tanto las letras como los espacios en blanco) se considera ideal. Para un trabajo de varias columnas, 40 a 50 caracteres es un buen promedio.

Podríamos necesitar una imagen a todo lo ancho de la fila dentro del contenedor, y bajo ella un párrafo centrado que utilice menos columnas en la medida que éstas se ensanchan junto a la pantalla, así mantener una anchura de párrafo cómoda a la lectura. El código del documento completo debería verse así:

```
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
    <title>Hola mundo</title>
  </head>
  <body>
  <div class="container">
   <div class="row">
    <div class="col-12">
     <img src="https://picsum.photos/1600/900?grayscale" class="w-100 my-4" alt="esta es una imagen random">
    </div>
    <div class="col-11 col-sm-10 col-md-9 col-lg-8 col-xl-7 col-xxl-6 mx-auto">
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla in molestie felis, eget egestas lacus. Etiam orci magna, dignissim at dolor eu, finibus molestie mi. Suspendisse fringilla sem magna, eget pharetra orci faucibus sit amet.</p>
    </div>
   </div>
  </div>    
  </body>
</html>
```

Una vez leído y comprendido el código en el ejemplo recién presentado, se puede pasar a la aplicación, donde se sumarán más elementos con clases y propiedades predefinidas con Bootstrap.

- - - - - - - 

## Aplicación

Vamos a tomar el código fuente de la página https://profesorfaco.github.io/infografia/clase-1/

Notarán que: 

- se indican varios niveles de título, pero se usa una única vez el `h1`

- se rellena con [Loren Ipsum](https://www.lipsum.com/)

- se usan imágenes de relleno, que ustedes podrían cambiar con sus bocetos (dejándolas con un nombre sin tildes, acentos ni espacios, y un peso bajo los 250kb con Photoshop, [Squoosh](https://squoosh.app/) o [TinyPNG](https://tinypng.com/))

Una vez modifiquen el código fuente de la página con algunos títulos, párrafos e imágenes, vamos a crear un [repositorio en GitHub](https://docs.github.com/es/repositories/creating-and-managing-repositories/about-repositories) y un [sitio de página de GitHub](https://docs.github.com/es/pages/getting-started-with-github-pages/creating-a-github-pages-site). Para ambas cosas, necesitan [su propia cuenta](https://github.com/signup) en [GitHub](https://github.com/).

- - - - - - - 

###### [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-2) 
