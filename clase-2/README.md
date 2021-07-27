# Infografía digital: HTML, SVG y CSS

### Clase 2 → Jueves 7 de octubre, 2021

- - - - - - - 

## Presentación

Ya aprendimos que **HTML (HyperText Markup Language) es un lenguaje estándar que describe la estructura de las páginas web (qué es lo que contiene la página)**. Este se complementa con otro lenguaje estándar, el **CSS (Cascading Style Sheets) que describe la presentación de las páginas web (cómo se muestra lo que contiene la página)**. 

Ahora corresponde aprender sobre un "primo hermano" del HTML, el **SVG (Scalable Vector Graphics)** que es un lenguaje estándar, basado en [XML](https://es.wikipedia.org/wiki/Extensible_Markup_Language), que describe gráficos vectoriales. Esta descripción se basa en las formas que lo componen, sus atributos y transformaciones. Nos referimos a formas tales como lineas simples, líneas quebradas, círculos, elipses, rectángulos, polígonos simples y trazados complejos, que respectivamente se describe con las etiquetas:

```
<line x1="0" y1="0" x2="200" y2="200" />

<polyline points="20,20 40,25 60,40 80,120 120,140 200,180" />

<circle cx="50" cy="50" r="40" />

<ellipse cx="200" cy="80" rx="100" ry="50" />

<rect width="300" height="100" />

<polygon points="200,10 250,190 160,210" />

<path d="M150 0 L75 200 L225 200 Z" />
```

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

El tercer ejemplo toma algo de los dos anteriores. Se trata de un elemento HTML `<img>` cuyo atributo no va por un recurso independiente, sino que aprovecha su propia data (que es código SVG con un ajuste en los signos `<` y `>`).

- - - - - - - 

## Exploración

Pendiente.

- - - - - - - 

## Aplicación

Pendiente.

- - - - - - - -

###### [← CLASE PASADA](https://github.com/profesorfaco/infografia/tree/main/clase-1) — [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-3) 
