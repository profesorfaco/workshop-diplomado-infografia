# HTML, SVG, CSS y JavaScript

### Clase 3 → 25-11-2021

- - - - - - - 

#### Presentación

Ya revisamos HTML, SVG y CSS. Aprendimos que HTML describe, mediante elementos, páginas web. Su primo hermano, el SVG, hace lo mismo con gráficos vectoriales. Tambien aprendimos que CSS puede describir, mediante reglas, el aspecto de tales páginas y gráficos vectoriales. 

Para avanzar rápido en la definición del aspecto de páginas que deben ser *responsivas*, estamos aprovechando [el CSS de Bootstrap](https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.css).

En esta clase corresponde dar un paso que nos llevará desde lenguajes de descripción a un lenguaje de programación.

**JavaScript es un lenguaje de programación con el que las páginas web se hacen interactivas, por vía del control del navegador web y su Modelo de Objetos de Documento ([DOM; Document Object Model](https://es.wikipedia.org/wiki/Document_Object_Model))**.

Este control no re-escribe. Lo que ya fue escrito en HTML, SVG o CSS se quedará como está. Lo que se controla es la "comprensión de la lectura ya hecha" por el navegador web. Por este motivo pueden haber diferencias entre un **ver código fuente** y un **inspector de elementos**.

- - - - - - - 

#### Exploración

Para ver diferencias entre un **ver código fuente** y un **inspector de elementos**, por favor copien el siguiente código y péguenlo en Atom o Sublime Text, para luego guardarlo con extensión `.html` y abrirlo en un navegador web:

```
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>¡JavaScript!</title>
  </head>
  <body>
    <button id="unique">Soy un botón</button>
    <script>
    	var b = document.getElementById("unique");
    	b.addEventListener("click", function(){
    	alert("¡Un mensaje de alerta!")
    	}, false);
    	b.insertAdjacentHTML("beforebegin", "Hola ");
    </script>
  </body>
</html>
```

En su navegador web revisen el código fuente, y noten que no existe un "Hola" antes del `<button id="unique">Soy un botón</button>`.

Revisando las partes del código recién escrito, entre `<script></script>`, tenemos:

- `var` anteciendo a `b`: Estoy creando una variable a la que le llamo, simplemente, b. Pueden imaginar una caja que tenga una b. También podría crear una variable [con `let` y `const`](https://medium.com/@tatymolys/var-let-y-const-donde-cuando-y-por-qu%C3%A9-d4a0ee66883b).

- `=` siguiendo a `b`: Estoy asignando a la variable recién creada un valor. Pueden imaginar que estoy guardando en esa caja algo, y luego llamaré a ese algo por el nombre de la caja que lo contiene. 

- `document.getElementById("unique")`: En el documento ya interpretado por el navegador, quiero que se busque aquello que tenga identidad "unique".

- `b.addEventListener("click", function(){}, false)`: Le aviso a la máquina que quede atenta al click en aquello que dejé guardado en `b`, y en caso hay un click se ejecutará una función.

- `b.insertAdjacentHTML("beforebegin", "Hola ")`: Nuevamente tomo la caja imaginaria, para agregar un contenido como HTML. Pero en el código fuente NO hay un "Hola" escrito, aunque lo podrás ver (esta es la diferencia entre lo efectivamente escrito en el código fuente y la comprensión de lectura a la vista en la inspección de elementos).

La manera en que se escriban las instrucciones puede variar dependiendo de la lógica de la misma instrucción, el estándar que se está respetando, (1) las (malas)costumbres de quien progreme, la biblioteca (*library*) de JavaScript en que nos apoyemos o el marco de trabajo (*framework*) de JavaScript en que nos basemos.

1. Un ejemplo de (mala)costumbre: En el ejemplo usé `document.getElementById("unique")` cuando ya podría estar usando `document.querySelector("#unique")`. Si no tuviera esa (mala)costumbre evitaría problemas confundiendo `document.getElementById()`, `document.getElementsByClassName()` o `document.getElementsByTagName()`.

2. ¿Qué es una *library* de JavaScript? Es código preparado y explicado, que permite resolver cosas específicas, como un gráfico o un mapa. Con una analogía cocinera: una biblioteca es como una sopa Maggi. 

3. ¿Qué es un *framework* de JavaScript? También es código preparado y explicado. La diferencia es que permite resolver cosas grandes, como una aplicación web completa (ver vue.js y react.js). Si adaptamos la analogía de la cocina, en un framework tenemos una selección de ingredientes listos, que nos permitirán hacer muchísismo más que  sopa.

¿Por qué usar *libraries* o *frameworks*? Porque los requerimiento de interacción son cada vez más complejos, y las dinámicas del trabajo tienden al [Software funcionando tan rápido como sea posible](https://agilemanifesto.org/iso/es/manifesto.html).

¿Usaremos algunos? Podríamos ver alguna biblioteca la próxima clase, pero, por ahora, vamos a resolver algunas cosas sin ellas: moviéndonos en espacios de interacción sencillos.

- - - - - - - 

#### Aplicación

https://profesorfaco.github.io/infografia/clase-3/

- - - - - - - -

###### [← CLASE PASADA](https://github.com/profesorfaco/infografia/tree/main/clase-2) — [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-4) 
