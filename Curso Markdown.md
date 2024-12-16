# **CURSO MARKDOWN**

# Esto es un encabezado de nivel 1 (hay 6)
## Esto es un encabezado de nivel 2
### Esto es un encabezado de nivel 3
#### Esto es un encabezado de nivel 4
##### Esto es un encabezado de nivel 5
###### Esto es un encabezado de nivel 6
(Se necesita dejar un espacio entre los gatos y el encabezado)

**Nota:** los encabezados también funcionan como anclas internas

## Parrafos
Esto es un párrafo común y corriente. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Cursiva y negrita
Palabra en _cursiva_

Palabra en **negrita**

**_Cursiva y negrita_**

***cursiva y negrita***

___cursiva y negrita___

## Tachar texto
Podemos tachar texto con el caracter ~ (Alt + 1 2 6)
Palabra ~~tachada~~

## Resaltado en color
Depende del interprete de markdown, podemos ver las palabras entre doble jugeo de simbolos de igual, subrayadas de un color

==resaltado==

## Enlaces
Se definen con unos corchetes donde ira el texto a mostrar y en seguida unos parentesis donde va el link, si queremos usar una ancla interna, en el parentesis va el simbolo de # seguido de la ancla, si esta ancla tiene varias palabras, usamos guion medio en vez del espacio

[Instagram](https://www.instagram.com/kobra_gloryg/)

[Ir a Encabezado 1](#esto-es-un-encabezado-de-nivel-1-hay-6)

Tambien podemos hacer una lista de enlaces y mostrar texto en su hover de la siguiente manera

[Enlace 1][1], [Enlace 2][2], [Enlace 3][3]

[1]: http://joedicastro.com/consejos
[2]: http://joedicastro.com/consejos "Consejos"
[3]: http://joedicastro.com/

O como un enlace muy sencillo solo encerramos la url en los simbolos menor y mayor que

<http://joedicastro.com>

## Enlaces entre notas
Esto depende mucho del interprete, por ejemplo en obsidian podemos insertar enlaces que nos redirijan a otra nota u otro archivo .md usando un juego de corchetes con el texto a mostrar y despues un par de parentesis con el nombre del archivo y si el archivo tiene espacios en su nombre, en vez del espacio ponemos %20 

[Otra nota](Otra%20nota.md)

O tambien podemos defenir este tipo de enlaces con doble corchete anidado, en este formato solo ponemos el nombre del archivo tal cual sin el .md

[[Otra nota]]

## Imagenes
Parecido a los enlaces, para las imagenes necesitamos un signos de exclamacion, despues un juego de corchetes y en seguida un par de parentesis, en los corchetes va el nombre que le querramos dar a la imagen (alt) y en los parentesis la ruta de la imagen, ya sea local o externa

Nota: Tambien podemos hacer listas de imagenes como lo hacemos con los enlaces

![Manuel Instagram Perfil](https://jonmircha.com/img/blog/this-is-javascript.jpg)

Para redimensionar la imagen, despues del nombre de imagen ponemos | y el numero en pixeles (Esto depende del interprete)

![Manuel Instagram Perfil|100](https://jonmircha.com/img/blog/this-is-javascript.jpg)

## Divisiones
Las divisiones son lineas horizontales que nos ayudan a separar contenido, estas las declaramos por tres guiones medios

Antes de la division

---

Despues de la division

## Listas
Para una lista ordenada necesitamos poner el numero uno, punto, espacio y ya el texto, podriamos poner numeros ascendentes como en cualquier otra lista (1., 2., 3., ...), pero con poner "1. " markdown hace la notacion ascendente sin importar cuantos elementos conformen la lista
1. Item 1
1. Item 2
1. Item 3

Para listas de viñetas usamos el asterisco
* item 1
* item 2
* item 3

Para listas de viñetas tambien podemos usar el guion medio
- item 1
- item 2
- item 3

Para trabajar sublistas necesitamos el uso de la identación
* item 1
    * item 1.1
* item 2
    * item 2.1
* item 3
    * item 3.1

Tambien podemos hacer listas de tareas con guion medio y corchetes con un espacio dentro, para dejar una seleccionada ponemos una x dentro de los corchetes (Esto depende del interprete)
- [ ] tarea 1
- [ ] tarea 2
- [x] tarea 3

## Citas
Para hacer citas hacemos uso del simbolo mayor que, esto para una cita de linea
> Extraño al barrio pero mis sueños estan fuera de el. - Manuel R.S.

Para hacer citas de bloque usamos el simbolo mayor que en todas las lineas usadas
> Hay tres cosas que no se pueden ocultar,
>
> el sol, la luna y la verdad.
>
> Teen golf

## Tablas
Para hacer tablas hacemos uso del simbolo pipe "|" como bordes verticales de nuestra tabla y despues de los titulos usamos | acompañado de tres guiones medios por cada celda
Nota: No es necesario alinear las celdas y su contenido para que en modo edicion parezca una tabla, markdown la interpreta si esta o no alineada

| Nombre    | Edad | Correo              |
| --------- | ---- | ------------------- |
| Manuel    | 21   | manuel@gmail.com    |
| Alejandro | 20   | alejandro@gmail.com |

Se puede especificar la alineación de cada columna mediante la adición de dos puntos a las líneas de separación. Dos puntos a la izquierda de la línea de separación hará que la columna esté alineada a la izquierda, dos puntos a la derecha de la línea hará que la columna esté alineada a la derecha, dos puntos en ambos lados significa que la columna se alinea al centro.

| Elemento | Cantidad | Precio |
| :------- | :------: | -----: |
| Item 1   | 15       | 150€   |
| Item 2   | 3250     | 23,65€ |

## Codigos
Para codigo en linea usamos acentos graves

La siguiente palabra `let` la usamos para definir una variable con scope local en js

Para codigo en linea usamos tres acentos graves al inicio y al final del bloque de codigo, podemos especificar el lenguaje usado poniendo el nombre del lenguaje de programacion usado en el bloque despues de los primeros acentos

```js
const sumar = nombre => {
    console.log(`Hola ${nombre}`);
}
```

## Código HTML
Podemos escribir etiquetas HTML en markdown
<form>
    <label for="name">Nombre</label>
    <input type="text" id="name" placeholder="Escribe tu nombre..."></input>
</form>

## Comentarios
Para hacer un comentario en markdown es de la misma manera que en HTML o con dos simbolos de porcentaje al inicio y al final del comentario (este ultimo puede variar dependiendo del interprete)
<!-- Esto es un comentario -->
%% Esto es un comentario %%

## Ignorar sintaxis de markdown
Para ignorar caracteres que forman una sintaxis en markdown anteponemos una diagonal invertida en cada uno de estos caracteres

Palabra en \*\*negrita\*\*

