# Infografía digital: HTML, SVG y CSS

### Clase 2 → Jueves 7 de octubre, 2021

- - - - - - - 

## Presentación

Ya aprendimos que **HTML (HyperText Markup Language) es un lenguaje estándar que describe la estructura de las páginas web (qué es lo que contiene la página)**. Este se complementa con otro lenguaje estándar, el **CSS (Cascading Style Sheets) que describe la presentación de las páginas web (cómo se muestra lo que contiene la página)**. 

Ahora corresponde aprender sobre "primo hermano" del HTML: El **SVG (Scalable Vector Graphics)**. Con este lenguaje se describen gráficos vectoriales (qué formas los componen y cuáles son sus atributos). 

En los gráficos vectoriales podemos encontrarnos con lineas rectas, líneas quebradas, círculos, elipses, rectángulos, polígonos simples y trazados complejos, formas que serán descritas con los atributos correspondientes a su geometría:

```
<line x1="0" y1="0" x2="200" y2="200" />

<polyline points="20,20 40,25 60,40 80,120 120,140 200,180" />

<circle cx="50" cy="50" r="40" />

<ellipse cx="200" cy="80" rx="100" ry="50" />

<rect width="300" height="100" />

<polygon points="200,10 250,190 160,210" />

<path d="M150 0 L75 200 L225 200 Z" />
```

Estas formas también pueden ser afectas mediante CSS, con propiedades particulares, distintas de las que afectan al hipertexto (del HTML), así, por ejemplo, podría agregar la clase `enrojecido` como atributo en un círculo, y este se pintaría de rojo con un borde negro de 1 pixel de ancho. 

```
.enrojecido{
  fill: red;
  stroke:black;
  stroke-width:1px;
}
```

No confundamos las propiedades `fill` y `stroke` con `color` y `border`; las dos primeras pueden afectar al SVG, mientras que las dos últimas pueden afectar al HTML.

Los gráficos descritos por SVG pueden escalar para ajustarse a diferentes resoluciones de pantalla, sin pérdida de resolución, y se pueden incluir en una página web de manera directa (como código SVG) o vinculada (como documento SVG).

Examinemos un primer ejemplo: 

```
<svg xmlns="http://www.w3.org/2000/svg" width="100" height="100" viewBox="0 0 100 100">
<circle cx="50" cy="50" r="40"/>
</svg>
````

En el primer ejemplo tenemos un elemento `svg` que establece un sistema de coordenadas. Este `svg` es el elemento más externo de cualquier documento SVG, pero también puede ser usado para agregar un fragmento de un SVG dentro de un documento SVG o HTML.

Segundo ejemplo: 

```
<object data="grafica.svg" type="image/svg+xml" />
```

En el segundo ejemplo tenemos el elemento HTML `<object>`, que representa un recurso externo que puede ser tratado como una imagen, un contexto de navegación anidado, o como un recurso que debe ser manejado por un plugin. La data correspondería a un documento SVG independiente (que solo contendría lo del primer ejemplo).

Un tercer ejemplo: 

```
<img src="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='100' height='100' viewBox='0 0 100 100'%3E%3Ccircle cx='50' cy='50' r='40'/%3E%3C/svg%3E">
```

El tercer ejemplo toma algo de los dos anteriores. Se trata de un elemento HTML `<img>` cuyo atributo de recurso (`src`) no va por un archivo independiente, sino que aprovecha su propia data (que es código SVG con un ajuste en las comillas, siempre simples entre dobles, y los signos `<` y `>`, que son reemplazados por`%3C` y `%3E` respectivamente).

- - - - - - - 

## Exploración

Pendiente.

- - - - - - - 

## Aplicación

Pendiente.

- - - - - - - -

###### [← CLASE PASADA](https://github.com/profesorfaco/infografia/tree/main/clase-1) — [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-3) 
