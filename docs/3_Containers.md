# Elementos a nivel de bloque y en línea

## Visión general

Como vimos en nuestro primer curso, los párrafos (`<p>`) contienen un bloque de texto.
Sin embargo, podemos usar contenedores para agrupar varios elementos.

### Elementos a nivel de bloque

Un elemento de nivel de bloque siempre comienza en una nueva línea y ocupa todo el ancho disponible (se extiende a la izquierda y a la derecha hasta donde puede).

El elemento `<div>` es un elemento de nivel de bloque.

#### div

El elemento `<div>` se utiliza a menudo como contenedor de otros elementos HTML.
No hay atributos requeridos, pero el estilo, la clase y la identificación son comunes.

Ejemplo 1:

```html
<div>
	<p>Este es mi primer contenedor div!</p>
	<img
		src="..\Images\DSC_1442.jpg"
		width="600"
		height="800"
		alt="DSC_1442.jpg"
	/>
</div>
```
><div>
> <p>Este es mi primer contenedor div!</p>
> <img src="..\Images\DSC_1442.jpg"	width="600"	height="800" alt="DSC_1442.jpg"/>
> </div>

Resultado:


El ejemplo anterior crea un contenedor "div" con un párrafo y una imagen.

Un contenedor puede contener, como cualquier otro elemento HTML, atributos de estilo. Todos los elementos hijos de ese contenedor heredarán este estilo, a menos que se sobreescriba en un elemento específico.

Ejemplo:

```html
<div style="background-color: beige" id="MiPrimerContenedor">
	<p>Aquí está el color de fondo beige.</p>
	<p style="background-color: purple;color: white;">Aquí está el color de fondo púrpura y texto blanco.</p>
</div>
```

Resultado:
> <div style="background-color: beige" id="MiPrimerContenedor">
> <p>Aquí está el color de fondo beige.</p>
> <p style="background-color: purple;color: white;">Aquí está el color de fondo púrpura y texto blanco.</p>
> </div>

El ejemplo anterior muestra de un contenedor `<div>` que contiene 2 párrafos y una identificación.
El atributo de estilo en el `<div>` pondrá el color de fondo en beige para todos los elementos subyacentes.
En el caso de nuestro segundo párrafo, el color de fondo se sobreescribe y se mostrará como púrpura.

### Elementos a nivel de línea

Un elemento en línea no comienza en una nueva línea y sólo ocupa el ancho necesario, como el elemento `<span>`.

#### span

El elemento `<span>` es un contenedor en línea que se utiliza para marcar una parte de un texto, o una parte de un documento.
No hay atributos requeridos, pero el estilo, la clase y la identificación son comunes.
Cuando se usa junto con el CSS, el elemento `<span>` puede ser usado para dar estilo a partes del texto.

Ejemplo:
```html
<p>Mi mamá tiene ojos <span style="color:blue;font-weight:bold">azules</span> y mi papá tiene ojos <span style="color:darkolivegreen;font-weight:bold">verdes oscuros</span>.</p>
```

Resultado:
> <p>Mi mamá tiene ojos <span style="color:blue;font-weight:bold">azules</span> y mi papá tiene ojos <span style="color:darkolivegreen;font-weight:bold">verdes oscuros</span>.</p>

## Resumen

* Hay dos valores de visualización: en bloque y en línea
* Un elemento de nivel de bloque siempre comienza en una nueva línea y ocupa todo el ancho disponible
* Un elemento en línea no comienza en una nueva línea y sólo ocupa el ancho necesario
* El elemento `<div>` es un nivel de bloque y se usa a menudo como contenedor de otros elementos HTML
* El elemento `<span>` es un contenedor en línea usado para marcar una parte de un texto, o una parte de un documento

\
[Volver a la vista general](index.md)
