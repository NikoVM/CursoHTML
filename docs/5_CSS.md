# CSS

## Visión general

### ¿Qué es el CSS?

Las Hojas de Estilo en Cascada (CSS) se utilizan para dar formato al diseño de una página web.

Con CSS, puedes controlar el color, la fuente, el tamaño del texto, el espacio entre elementos, cómo se posicionan y disponen los elementos, qué imágenes de fondo o colores de fondo se deben utilizar, diferentes pantallas para diferentes dispositivos y tamaños de pantalla, ¡y mucho más!

> :warning: Importante
>
>
> La palabra "en cascada" significa que un estilo aplicado a un elemento padre también se aplicará a todos los elementos hijos dentro del padre. Por lo tanto, si establece el color del cuerpo de texto en "azul", todos los encabezados, párrafos y otros elementos de texto dentro del cuerpo también obtendrán el mismo color (a menos que especifique algo más)!

### Usando CSS

El CSS puede ser añadido a los documentos HTML de 3 maneras:

-   En línea - usando el atributo de estilo dentro de los elementos HTML
-   Interno - usando un elemento de <estilo> en la sección de <cabeza>
-   Externo - usando un elemento <link> para enlazar a un archivo CSS externo

La forma más común de añadir CSS, es mantener los estilos en archivos CSS externos. Sin embargo, en este tutorial usaremos estilos en línea y estilos internos, porque esto es más fácil de demostrar, y más fácil para que lo pruebes tú mismo.

## CSS en línea

Un CSS en línea se utiliza para aplicar un estilo único a un solo elemento HTML.
Un CSS en línea utiliza el atributo style de un elemento HTML.
El siguiente ejemplo establece el color de texto del elemento `<h1>` en azul, y el color de texto del elemento `<p>` en rojo:

```html
<h1 style="color:blue;">Un encabezado azul</h1>

<p style="color:red;">Un párrafo rojo</p>
```

Resultado:

> <h1 style="color:blue;">Un encabezado azul</h1>
> <p style="color:red;">Un párrafo rojo</p>

## CSS interno

Un CSS interno se utiliza para definir un estilo para una sola página HTML.
Un CSS interno se define en la sección `<head>` de una página HTML, dentro de un elemento `<style>`.
El siguiente ejemplo establece el color de texto de TODOS los elementos `<h1>` (en esa página) en azul, y el color de texto de TODOS los elementos `<p>` en rojo. Además, la página será mostrada con un color de fondo "azul polvo":

```html
<!DOCTYPE html>
<html>
	<head>
		<style>
			body {
				background-color: powderblue;
			}
			h1 {
				color: blue;
			}
			p {
				color: red;
			}
		</style>
	</head>
	<body>
		<h1>Este es un título</h1>
		<p>Este es un párrafo</p>
	</body>
</html>
```

Resultado:

<div style="background-color: powderblue;">
    <h1 style="color: blue;">Este es un título</h1>
    <p style="color: red;">Este es un párrafo.</p>
</div>

## CSS externo

Se utiliza una hoja de estilo externa para definir el estilo de muchas páginas HTML.
Para utilizar una hoja de estilo externa, añada un enlace a la misma en la sección `<head>` de cada página HTML.

Página HTML:

```html
<!DOCTYPE html>
<html>
	<head>
		<link rel="stylesheet" href="styles.css" />
	</head>
	<body>
		<h1>Este es un título</h1>
		<p>Este es un párrafo.</p>
	</body>
</html>
```

Página CSS:

```css
body {
	background-color: powderblue;
}
h1 {
	color: blue;
}
p {
	color: red;
}
```

Resultado:

<div style="background-color: powderblue;">
    <h1 style="color: blue;">Este es un título</h1>
    <p style="color: red;">Este es un párrafo.</p>
</div>

> :point_up: Consejo
>
>
> Con una hoja de estilo externa, puedes cambiar el aspecto de un sitio web entero, ¡cambiando un fichero!

## Propiedades CSS comúnmente utilizadas

### Colores, fuentes y tamaños del CSS

La propiedad `color` CSS define el color del texto a ser usado.
La propiedad `font-family` de CSS define la fuente que se va a utilizar.
La propiedad `font-size` de CSS define el tamaño del texto que se va a usar.

```css
h1 {
	color: blue;
	font-family: verdana;
	font-size: 300%;
}
p {
	color: red;
	font-family: courier;
	font-size: 160%;
}
```

Resultado:

<div style="background-color: powderblue;">
    <h1 style="color: blue;font-family: verdana;font-size: 300%;">Este es un título</h1>
    <p style="color: red;font-family: courier;font-size: 160%;">Este es un párrafo.</p>
</div>

### Borde del CSS

La propiedad `border` de CSS define un borde alrededor de un elemento HTML y contiene 3 argumentos.

1. El grosor del borde
2. El estilo del borde
3. Cualquier color

> :point_up: Consejo
>
>
> Puedes definir un borde para casi todos los elementos HTML.

Ejemplo:

```css
p {
	border: 2px solid powderblue;
}
```

Resultado:

<div>
	<p style="border: 2px solid powderblue">Mi primera borde</p>
</div>

### Relleno de CSS

La propiedad `padding` de CSS define un relleno (espacio) entre el texto y el borde.
Ejemplo:

```css
p {
	border: 2px solid powderblue;
	padding: 30px;
}
```

Resultado:

<div>
	<p style="border: 2px solid powderblue; padding: 30px;">Mi primera borde</p>
</div>

En el ejemplo anterior, sólo pusimos un argumento para el "acolchado". Podemos dar hasta 4 argumentos, dependiendo de los diferentes rellenos por nivel, como se muestra en el ejemplo siguiente.

```css
/* Aplicar a los cuatro lados */
padding: 1em;

/* Vertical | horizontal */
padding: 5% 10%;

/* Arriba | horizontal | abajo */
padding: 1em 2em 2em;

/* Arriba | derecha | abajo | izquierda */
padding: 5px 1em 0 2em;
```

### Margen CSS

La propiedad `margin` de CSS define un margen (espacio) fuera del borde.

Ejemplo:

```css
p {
	border: 2px solid powderblue;
	margin: 50px;
}
```

Resultado:

<div>
	<p style="border: 2px solid powderblue; margin: 50px">Mi primera borde</p>
</div>

Al igual que con la propiedad `padding`, podemos dar de 1 a 4 argumentos para definir el espacio.

### Usando el atributo de clase de CSS

El atributo de `class` se utiliza a menudo para señalar un nombre de clase en una hoja de estilo.

Usando el atributo class, puedes diferenciar en estilo para las mismas etiquetas HTML.
Por ejemplo, un párrafo con la clase "importante" tiene un color de texto rojo, un párrafo con la clase "información" se muestra en azul.
Una clase en CSS se define añadiendo un punto delante del nombre de la clase.

En HTML:

```html
<!DOCTYPE html>
<html>
	<head>
		<title>El atributo de clase</title>
	</head>
	<body>
		<p class="importante">Soy importante y se me mostrará en rojo</p>
		<p class="informacion">Soy informativo y se me muestra en azul</p>
	</body>
</html>
```

En CSS:

```css
.importante {
	color: red;
}
.informacion {
	color: blue;
}
```

Resultado:
<p style="color:red">Soy importante y se me mostrará en rojo</p>
<p style="color:blue">Soy informativo y se me muestra en azul</p>

\
[Volver a la vista general](Index.html)
