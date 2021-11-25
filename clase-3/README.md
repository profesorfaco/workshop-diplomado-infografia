# HTML, SVG, CSS y JavaScript

### Clase 3 → 25-11-2021

- - - - - - - 

#### Presentación

Ya revisamos HTML, SVG y CSS. Aprendimos que HTML describe, mediante elementos, a las páginas web. Su primo hermano, el SVG, hace lo mismo con los gráficos vectoriales. Tambien aprendimos que CSS puede describir, mediante reglas, el aspecto de páginas y gráficos vectoriales. 

Para avanzar rápido en la definición del aspecto de páginas que deben ser *responsivas*, estamos aprovechando [el CSS de Bootstrap](https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.css).

En esta clase corresponde dar un paso que nos llevará desde lenguajes de descripción a un lenguaje de programación.

**JavaScript es un lenguaje de programación con el que las páginas web se hacen interactivas, por vía del control del navegador web y su Modelo de Objetos de Documento ([DOM; Document Object Model](https://es.wikipedia.org/wiki/Document_Object_Model))**.

Este control no re-escribe. Lo que ya fue escrito en HTML, SVG o CSS se quedará como está. Lo que se controla es la "comprensión de la lectura ya hecha" por el navegador web. Por este motivo pueden haber diferencias entre un **ver código fuente** y un **inspector de elementos**.

- - - - - - - 

#### Exploración

Para encontrar las diferencias entre un **ver código fuente** y un **inspector de elementos**, por favor copien el siguiente código y péguenlo en Atom o Sublime Text, para luego guardarlo con extensión `.html` y abrirlo en un navegador web:

```
<!doctype html>
<html lang="es">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>¡JavaScript!</title>
  </head>
  <body>
    <button id="especial">Soy un botón</button>
    <script>
    	var x = document.getElementById("especial");
    	x.addEventListener("click", function(){
    	alert("¡Un mensaje de alerta!")
    	}, false);
    	x.insertAdjacentHTML("beforebegin", "Hola ");
    </script>
  </body>
</html>
```

En su navegador web revisen el código fuente, y noten que no existe un "Hola" antes del `<button id="especial">Soy un botón</button>`, aun cuando pueden verlo por el control de la "comprensión de la lectura".

Para comprender las instrucciones entre `<script></script>`, podemos prestar atención a:

- **La `x` después de `var`**. Allí se crea una variable de nombre `x`. Además de [`var`, podríamos usar `let` o `const`](https://medium.com/@tatymolys/var-let-y-const-donde-cuando-y-por-qu%C3%A9-d4a0ee66883b). Pueden imaginar que al usar `var`, `let`o `const` se crea una caja vacía, con su nombre marcado: En este caso, marcada con una `x`.

- **El signo `=` después de `x`**. Así se asigna a la variable recién creada un contenido. Pueden imaginar que estoy guardando algo en esa caja, y luego llamaré a ese algo por el nombre de la caja que lo contiene. Importante es agregar que en JavaScript lo igual es `==` y lo diferente es `!=`. Pero un único signo `=` es asignación de contenido (el algo de la caja marcada con `x` será tal cosa).

- **El `document.getElementById("especial")`**. De lo ya intepretado por el navegador, quiero tomar aquello que tenga la identidad `especial`.

- **Las tres líneas que incluyen el `x.addEventListener("click", function(){}, false)`**. Le aviso al navegador que se disponga a escuchar el `click` de aquello que dejé guardado en `x`, y que corra una función si se hace tal `click`.
 
- **El cierre con `x.insertAdjacentHTML("beforebegin", "Hola ")`**. Antes de terminar, vuelvo a tomar la caja marcada con la `x`, para que se inserte, antes suyo, un "Hola".

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
