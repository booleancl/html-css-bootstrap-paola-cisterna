# HTML CSS BOOTSTRAP

Html CSS y Javascript son los pilares de toda aplicación o sitio web. Cualquier cosa que funcione dentro de un navegador web (chrome, mozilla, safari) utiliza estos pilares. Y no solo eso, hoy también se pueden hacer aplicaciones "nativas" con estas tecnologías.

## HTML

Significa **Hyper Text Markup Language**, que en castellano sería algo como Lenguaje de marcado de hyper texto. Lenguaje de marcado es por la *Etiquetas*. Dependiendo de su etiqueta el navegador lo procesa de diferente forma. Y el hyper texto se refiere a que estos documentos están enlazados por *links*.

Con HTML crearemos *documentos estructurados* mediante etiquetas que el navegador puede interpretar.

El documento principal de un sitio o aplicación de debe llamar **index.html**. Todo junto y en minúsculas.

### Doctype

Esta primera etiqueta indica al navegador la versión de HTML. En este caso indica que es la versión 5.
```html
  <!DOCTYPE html>
```

### html
Luego de eso viene la primera etiqueta que es parte del documento. la famosa etiqueta **html**:
```html
<html lang="es">
  ...
</html>
```

Del ejemplo anterior vemos que esta etiqueta se compone de 2 partes principales. La etiqueta de apertura `<html>` y la de cierre `</html>`.

Entremedio de las etiquetas de apertura y cierre irá el contenido.

Además vemos la etiqueta de apertura tiene el **atributo** `lang="es"`, lo que le indica al navegador en qué idioma está el contenido del documento.

>**ATENCIÓN**: Solo las etiquetas de apertura pueden tener atributos, Las etiquetas de cierre no.

### head

A continuación viene etiqueta `head`. Esta etiqueta entrega información al **Navegador** sobre como visualizar el contenido que vendrá en las siguientes secciones. Por ejemplo se indica mediante etiquetas `meta` el set de caracteres que utilizará la página. Ejemplo:

```html
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hola Microsystem</title>
</head>
```

La tercera etiqueta `meta` que tiene el atributo `name="viewport"` permite que el contenido se cargue inicialmente considerando el tamaño de pantalla disponible, desde grandes a muy pequeños.

Además dentro del head se encuentra la etiqueta `title`, que es la encargada de mostrar el nombre del sitio en la pestaña del navegador.

Por otra parte dentro del `head` podemos cargar otros recursos que utilizará el documento como por ejemplo hojas de estilo CSS o archivos Javascript

### Estructura Jerárquica

Algo que es muy muy muy importante notar y que no es tan evidente, es que los documentos HTML forman una estructura jerárquica bien definida del tipo árbol. Donde la etiqueta raíz es la etiqueta `html`. Lo podemos visualizar de la siguiente forma

```html
  <html>
    <head></head>
    <body></body>
  </html>
``` 

Esto es muy importante de comprender ya que luego manejaremos las etiquetas pensando en su ubicación relativa dentro del árbol. Y pensaremos que las etiquetas son **nodos** que tienen **nodos padre**, **hermanos** y **nodos hijos**. 






la idea de los elementos no sematicos es utilizar css para darles estilo.
mas adelante, en este modulo veremos lo frecuente de uso el marco de trabajo o framework bootstrap.

## formacion 

contiene controles interactivos para ingresar informacion

´´´´html
<form action="/searc" method="get">
´´´´
</fors>
´´´´

### Etiquetas no semanticas

Estas etiquetas no tiene un significado propio y sirven como contenedor para agrupar otras etiquetasb 

## div

>´´´´html...

## spam

La etiqueta span se puede usar dentro del texto.

´´´´html
<div>
<p>Hola<span>mundo</span></p>
</div>
´´´´

La idea detras de los elementos no sematicos es utilizar css para darles estilo.

### Links

Los links son el corazon de internet y los crearemos frecuentemente. Se componen de el atributo 'href' que indica el destino del link y su contenido, que es lo que se muestra al usuario
´´´´html
<a href="heading.  html">Titulos</a>

### Imagenes 

Las imagenes son una 















### Unidades de medida 

En general, no solo en desarrollo, podemos clasificar las unidades de medida en dos grupos: 

Unidades Absolutas: pixel(px)
Unidades relativas: porcentaje,(%),rem,em,vh,uvw

#### rem 
Es una unidad de medida relativa al font-size del elemento raiz
#### em
Es relativa al font-size del mismo elemento
#### vh
Es relativo al 1% del alto de la pantalla (viewport)
#### vw
Es relativo al 1% del ancho de la pantalla o viewport


### Tipos de diseño 

- El diseño estatico: Sirve para un solo tamaño de pantalla 
- El diseño fluido: en porcentajes(%)
dependiendo del tamaño de la pantalla 
- El diseño responsivo:Tiene puntos de quiebre(distintos tamaños) para aplicar diferentes estilos 

### css MediaQueries
Utiliza la regla '@media' para incluir un bloque de propiedades css solo si la condicion es verdadera. Ejemplo:

´´´´css
 /* Extra small devices (phones, 600px and down) */
@media only screen and (max-width: 600px) {...}

/* Small devices (portrait tablets and large phones, 600px and up) */
@media only screen and (min-width: 600px) {...}

/* Medium devices (landscape tablets, 768px and up) */
@media only screen and (min-width: 768px) {...}

/* Large devices (laptops/desktops, 992px and up) */
@media only screen and (min-width: 992px) {...}

/* Extra large devices (large laptops and desktops, 1200px and up) */
@media only screen and (min-width: 1200px) {...} 

### display
@media only screen and (max-width: 600px){
    body{
      background-color: green
    }
    p{
        display: none;
    }
  }
  ```
El valor de la propiedad display modifica como el navegador posicionara la caja del elemento.
La caja puede ser de lado a lado, en ese caso la propiedad display tendrá el valor `block`.
Tambien podemos establecer el valor como `inline` y en ese caso, la caja sera del menor tamaño posible. Ejemplo:
```css







