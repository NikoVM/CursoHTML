# ¿Cómo se ve una página básica?

## Visión general

Todas las páginas HTML están construidas con elementos XML.

Un elemento consiste en una elemento de inicio, seguido por el contenido y luego la elemento final.
Una elemento comienza con "<" seguida de un nombre y termina con ">".
Ejemplo:

```xml
<Aron>
```

\
Una elemento de fin comienza con "</" seguido del mismo nombre del elemento de inicio, seguido de ">"
Ejemplo:

```xml
</Aron>
```

\
Cuando defines un elemento, defines su nombre y su contenido. El nombre se escribe entre "< >", el contenido se coloca dentro del elemento de inicio y fin.
Ejemplo:

```xml
<Aron>Es el mejor estudiante</Aron>
```

> :warning:     Importante
>
>
> Un elemento vacío puede mostrarse como:  
> ```xml 
> <Aron />
> ```

## elementos básicas reservadas

Puedes establecer cualquier nombre para una elemento XML, pero cuando trabajas en HTML, estás vinculado a varias elementos reservadas que están predefinidas.
A continuación, una lista de los elementos HTML más básicas y sencillas.

---

### `<!DOCTYPE html>`

Una página HTML siempre empezará definiendo su tipo de documento.
Todos los documentos HTML deben comenzar con una `<!DOCTYPE>` declaración.
La declaración no es una elemento HTML. Es una "información" para el navegador sobre qué tipo de documento esperar.
Ejemplo:
```html
<!DOCTYPE html>
```

---

### `<html>`

Después de definir el tipo de documento, siempre se empieza con el elemento `<html>`.
Ejemplo:
```html
<!DOCTYPE html>
<html>

</html>
```

---

### `<head>`

Contiene metadatos / información para el documento y se coloca dentro del elemento `<html>`.
Ejemplo:
```html
<!DOCTYPE html>
<html>
    <head>

    </head>
</html>
```
---

### `<title>`

Define un título para el documento y se coloca dentro del elemento `<head>`.
Ejemplo:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Título</title>
    </head>
</html>
```

---

### `<body>`

Define el cuerpo del documento y se coloca dentro del elemento `<html>`.
Ejemplo:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Título</title>
    </head>
    <body>
        El contenido de la página.
    </body>
</html>
```
> :warning:     Importante
>
>
> El elemento HTML contiene siempre 2 hijos: un elemento "head" para definir sus propiedades de encabezado y un elemento "body" que contiene el contenido de la página.
---

### `<p>`

Define un párrafo.
Ejemplo:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Título</title>
    </head>
    <body>
        <p>Este es un párrafo</p>
    </body>
</html>
```

---

### `<br />`

Inserta un solo salto de línea
Ejemplo:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Título</title>
    </head>
    <body>
        Esta es la primera línea.
        <br />
        Esta es la segunda línea.
    </body>
</html>
```
---

### `<hr />`

Inserta una línea horizontal en el contenido
Ejemplo:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Título</title>
    </head>
    <body>
        Añadiendo una línea horizontal,
        <hr />
        podemos separar el texto
    </body>
</html>
```

Resultado:

> Añadiendo una línea horizontal,
> <hr />
> podemos separar el texto

---

### `<h1>` ... `<h6>`

Los elementos de `<h1>` a `<h6>` se usan para definir los encabezados HTML.
\
`<h1>` define el encabezado más importante. `<h6>` define el encabezado menos importante.
> :point_up:     Consejo
> Sólo usa un `<h1>` por página - esto debería representar el encabezado/tema principal de toda la página.
> \
> Además, no se salte los niveles de encabezamiento - comience con `<h1>`, luego use `<h2>`, y así sucesivamente.

***

### Ejemplo completo
```html
<!DOCTYPE html>
<html>
	<head>
	    <title>Mi primera página web!</title>
	</head>
	<body>
            <p>Mi primera página web contiene un párrafo</p>
            <hr />
            <br />
            <p>Una línea de separación y una línea horizontal y un nuevo párrafo.</p>
	</body>
</html>
```
Resultado:
> <p>Mi primera página web contiene un párrafo</p>
> <hr />
> <br />
> <p>Una línea de separación y una línea horizontal y un nuevo párrafo.</p>

\
[Volver a la vista general](Index.md)
