# Atributos

Los atributos pueden ser genéricos (como para el texto de estilo) o específicos de un elemento (p.e. la fuente de una imagen).

* Todos los elementos HTML pueden tener atributos
* Los atributos proporcionan información adicional sobre los elementos
* Los atributos se especifican siempre en un elemento de inicio
* Los atributos suelen venir en pares nombre/valor como: nombre="valor"

## Atributos genéricos

### title
El atributo ``title`` define alguna información adicional sobre un elemento.
El valor del atributo title se mostrará como información de herramienta cuando pases el ratón por encima del elemento:

Ejemplo:
```html
<p title="Soy una información de herramienta">Este es un párrafo.</p>
```

### style
El atributo ``style`` se utiliza para añadir estilos a un elemento, como el color, la fuente, el tamaño y más.
Múltiples estilos están separados por un punto y coma.

Ejemplo 1:
```html
<p style="color:red;">Este es un párrafo rojo.</p>
```

Eemplo 2:
```html
<p style="color:blue;font-size: large;">Este es un párrafo azul con un tamaño de letra grande.</p>
```

## Atributos específicos

### href
Un elemento ``<a>`` define un hipervínculo. El atributo href especifica la URL de la página a la que va el enlace:

```html
<a href="https://www.w3schools.com">Visite W3Schools</a>
```

El ejemplo anterior apunta al hipervínculo https://www.w3schools.com. En la página web real, este hipervínculo se mostrará como "Visite W3Schools".

### src
Un elemento ``<img>`` se usa para incrustar una imagen en una página HTML. El atributo src especifica la ruta de la imagen que se va a mostrar:
```html
<img src="..\Images\DSC_1442.jpg">
```

### width y height
Un elemento ``<img>`` también debe contener los atributos de ancho (width) y alto (height), que especifican el ancho y el alto de la imagen (en píxeles):
```html
<img src="..\Images\DSC_1442.jpg" width="600" height="500">
```

### alt
El atributo ``alt`` requerido para un elemento ``<img>`` especifica un texto alternativo para una imagen, si la imagen por alguna razón no puede ser mostrada. Esto puede deberse a una conexión lenta, o a un error en el atributo src, o si el usuario utiliza un lector de pantalla.
```html
<img src="..\Images\DSC_1442.jpg" alt="Una leona durmiendo">
```

\
[Volver a la vista general](index.md)