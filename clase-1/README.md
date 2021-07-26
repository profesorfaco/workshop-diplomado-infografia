# Infografía digital: HTML y CSS

### Clase 1 → Martes 5 de octubre, 2021

- - - - - - - 

### Presentación
 
**HTML (HyperText Markup Language) es un lenguaje estándar que describe la estructura de las páginas web (qué es lo que contiene la página)**. 

HTML5 es la versión más reciente de este lenguaje. 

Lo más básico del HTML es el elemento. Cada elemento de HTML se escribe entre etiquetas: `<etiqueta>contenido</etiqueta>`; habiendo excepciones que no son más que una etiqueta, tales como la imagen (`<img>`), el quiebre de línea (`<br>`), la línea horizontal (`<hr>`) o el metadato (`<meta>`). 

Las etiquetas utilizan "[palabras reservadas](http://html5doctor.com/element-index/)" entre paréntesis angulares de apertura (`<`) y cierre (`>`).

En la primera o única etiqueta que conforma el elemento, antes que se cierre el paréntesis angular (`>`), se pueden agregar atributos que contienen información  acerca del elemento. 

En algunos casos el atributo aporta información adicional, como en un párrafo (`p`) con un atributo de clase (`class`) especial:

```
<p class="especial">Este es un párrafo</p>
```

Pero en otros casos el atributo aporta información clave, como en la definción del recurso (`scr`) que se despliega como imagen (`img`):

```
<img src="foto.jpg" alt="describe la foto">
```

Ahora observemos cómo los elementos estructuran un documento HTML:

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

- Un anuncio `<!doctype html>` que sigue un documento HTML en versión 5, así como una banderita en un sandwich puede anunciar la cadena de comida rápida donde se preparó.

- Un elemento `<html lang="es"></html>` que contiene a todo el documento HTML, que será escrito en español

- Un elemento `<head></head`> que contiene indicaciones que describen y complementan lo que se mostrará en la ventana del navegador.

- Un elemento `<body></body>` que contiene todo lo que se podría mostrar en la ventana del navegador.

Pero el documento HTML necesita una forma de verse distinta de la definida para el intercambio de trabajo científico en la Organización Europea para la Investigación Nuclear de 1989 (fondo blanco, letras negras, tipografía con serifa en tamaños predefinidos y vínculos subryados en azul cuando aún no han sido visitados). Para ello se complementa con CSS.

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

Para que no quede sin mencionarse, también se puede incluir CSS a nivel de atributos del HTML, pero esa es una forma poco eficiente porque afecta a un único elemento, el que lo contiene, y por lo mismo no utiliza selector: 

```
<a href="https://github.com/profesorfaco/infografia" style="color:red">este es un vínculo</a>
```

- - - - - - - 

#### Exploración

Pendiente

- - - - - - - 

#### Aplicación

Pendiente

- - - - - - - 

###### [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-2) 
