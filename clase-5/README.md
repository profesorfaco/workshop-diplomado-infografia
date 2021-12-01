# Infografía digital: Accesibilidad, usabilidad y rendimiento

### Clase 5 → 04-12-2021


- - - - - - - 

#### Presentación

**Hay un par de prueba rápidas que se puede hacer en cualquier página web**.

1. Si se está visitando la página con Chrome, se puede buscar en el menú la opción Editar > Voz > Empezar a hablar.

2. Si se está visitando la página con Firefox, se puede buscar en el menú la opción Ver > Estilo de página > sin estilo.

**Lo que resulte de 1 y 2, debería hacer sentido**.

**Para hacer una prueba más calmada, hay un par de servicios en línea que podrían aprovechar**:

1. Para revisar el código: https://validator.w3.org/nu/

2. Para revisar la accesibilidad: https://wave.webaim.org/

Ahora bien, **para hacer una auditoría completa**, que considere rendimiento, accesibilidad, buenas práctica de programación, SEO (Search Engine Optimization; posicionamiento en buscadores) y PWA (Progressive Web App), **podrías usar [LightHouse](https://developers.google.com/web/tools/lighthouse?hl=es)**.

Lighthouse genera reportes en dos versiones: [resumida](https://github.com/profesorfaco/infografia/tree/main/clase-5/reportes) o extendida.

Es probable que LightHouse dé indicaciones respecto del CCS, porque estamos aprovechando unas pocas líneas entre las muchísimas que ofrece Bootstrap. Consideren que Bootstrap ofrece [un estilo CSS muy grande](https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.css), de 11.266 líneas, que el navegador revisa completo antes de mostrar la página; y siempre conviene limitar las lecturas del navegador a lo estrictamente necesario. 

Para reducir el CSS a lo que realmente es aplicado, puede aprovecharse https://purifycss.online/ o algún otro truco explicado en https://css-tricks.com/how-do-you-remove-unused-css-from-a-site/

**Hasta aquí hemos considerado, principalmente, a las personas (acceso) y los navegadores (rendimiento) ¡Pero aún no consideramos a las máquinas!**

Las máquinas necesitan datos o, mejor dicho, metadatos. Con ellos pueden catalogar lo que ustedes publican en línea. Para cuidar los metadatos, es recomendable:

1. Hacer una revisión con https://www.heymeta.com/

2. Hacer una edición con https://megatags.co/ 

Al cuidar los [metadatos, cuidamos el posicionamiento en buscadores (SEO)](https://developers.google.com/search/docs/advanced/crawling/special-tags?hl=es)


- - - - - - - 

#### Exploración

Pendiente

- - - - - - - 

#### Aplicación

Pendiente

- - - - - - - -

###### [← CLASE PASADA](https://github.com/profesorfaco/infografia/tree/main/clase-4) — [CLASE SIGUIENTE →](https://github.com/profesorfaco/infografia/tree/main/clase-6) 
