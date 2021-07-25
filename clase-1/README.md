# Infografía digital: HTML y CSS

### Clase 1 → Martes 5 de octubre, 2021

- - - - - - - 

### Presentación
 
**HTML (HyperText Markup Language) es un lenguaje estándar que describe la estructura de las páginas web (qué es lo que contiene la página)**. 

HTML5 es la versión más reciente de este lenguaje. 

Lo más básico del HTML es el elemento. Cada elemento de HTML se escribe entre etiquetas: `<etiqueta>contenido</etiqueta>`; habiendo excepciones que no son más que una etiqueta, tales como la imagen (`<br>`), el quiebre de línea (`<br>`), la línea horizontal (`<hr>`) o el metadato (`<meta>`). 

Las etiquetas, sean dos o una, utilizan una [palabra reservada](http://html5doctor.com/element-index/) encerrada por paréntesis angulares de apertura (`<`) y cierre (`>`).

En la primera o única etiqueta que conforma el elemento, antes que se cierre el paréntesis angular (`>`), se pueden agregar atributos que contienen información  acerca del elemento. 

En algunos casos el atributo aporta información adicional, como en un párrafo (`p`) con un atributo de clase (`class`) especial:

```
<p class="especial">Este es un párrafo</p>
```

Pero en otros casos el atributo aporta información clave, como en la definción del recurso (`scr`) que se despliega como imagen (`img`):

```
<img src="foto.jpg" alt="describe la foto">
```

Con estos principios, podemos comenzar a observar la estructura de una página web: 

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

- Un anuncio `<!doctype html>` de que lo que sigue es un documento HTML en versión 5, así como una banderita en un sandwich puede anunciar la cadena de comida rápida donde se preparó.

- Un elemento `<html lang="es"></html>` contiene a todo el documento HTML, que será escrito en español

- Un elemento `<head></head`> contiene indicaciones que describen y complementan lo que se mostrará en la ventana del navegador.

- Un elemento `<body></body>` contiene todo lo que se muestra dentro de la ventana del navegador.

Podemos complementar esta breve introducción a HTML con una revisión de la página: https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/HTML_basics

**CSS (Cascading Style Sheets) es un lenguaje estándar que describe la presentación de las páginas web (cómo se muestra lo que contiene la página).**

CSS3 es la versión más reciente de este lenguaje. 

Lo más básico del CSS es la regla. Cada regla se inicia con un selector, seguido de paréntesis de llave `{…}`. Tal paréntesis contiene un bloque de declaraciones. En tal bloque, cada declaración se separa de otra mediante punto y coma `;`. Una declaración se compone del par `propiedad: valor`. Con todo lo dicho, una regla se escribirá, generalmente, de la siguiente manera: `selector{ propiedad: valor; }`

Podemos complementar esta breve introducción a CSS con una revisión de la página: https://developer.mozilla.org/es/docs/Learn/Getting_started_with_the_web/CSS_basics (no es necesario realizar el ejercicio que allí se propone).

- - - - - - - 

#### Exploración

Pendiente

- - - - - - - 

#### Aplicación

Pendiente

- - - - - - - 

###### [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-2) 
