# Curso básico de MarkDown

## **¿Qué es MarkDown?**

**Markdown** es un lenguaje de marcado ligero que se usa para dar formato a texto de manera sencilla y rápida. Se diseñó para que fuera fácil de leer y escribir en texto plano, pero que también pudiera convertirse en HTML u otros formatos.

### Características principales de MarkDown:

* Usa símbolos simples para dar formato al texto.
* Es compatible con muchas plataformas y herramientas, como GitHub, Jupyter Notebooks y editores de texto.
* Permite escribir documentos estructurados sin necesidad de conocer HTML.

### ¿Dónde se usa MarkDown?

- GitHub (README.md)
- Blogs y generadores estáticos
- Aplicaciones de documentación 
- Es el formato de la respuesta de inteligencias artificiales como ChatGPT

### Ventajas y desventajas

| Ventaja                          | Descripción                                                                                                                           |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Simplicidad y facilidad de uso   | No requiere aprender una sintaxis compleja <br> Más fácil de escribir que HTML o LaTeX                                                |
| Ligero y basado en texto plano   | No necesita software especial, cualquier editor de texto sirve <br> Archivos muy pequeños en comparación con documentos de Word o PDF |
| Amplia compatibilidad            | Se usa en GitHub, Notion, Jupyter Notebooks, blogs, documentación, etc. <br> Puede convertirse a HTML, PDF, LaTeX y otros formatos    |
| Legible incluso sin procesarlo   | Un archivo Markdown sin procesar sigue siendo entendible                                                                              |
| Fácil integración con HTML y CSS | Se puede combinar con HTML para personalizar el formato                                                                               |
| Ideal para documentación y notas | Usado en README.md, wikis y manuales técnicos                                                                                         |

| Desventaja                                            | Descripción                                                                                                                                                    |
| ----------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Opciones de formato limitadas                         | No tiene soporte nativo para fuentes, colores personalizados o diseño avanzado <br> Para estilos complejos, hay que usar HTML o CSS                            |
| No es un estándar único                               | Existen diferentes variantes como GitHub Flavored Markdown (GFM), CommonMark, etc. <br> Algunas características funcionan en unas plataformas pero no en otras |
| No es ideal para documentos grandes o complejos       | Para documentos con muchas secciones y gráficos avanzados, LaTeX o Word pueden ser mejores opciones                                                            |
| Depende de conversores para exportar a otros formatos | Para generar PDF o documentos bien formateados, se necesita Pandoc, Typora, etc.                                                                               |
| Soporte HTML restringido en algunas plataformas       | GitHub y otras plataformas bloquean ciertas etiquetas HTML por seguridad                                                                                       |

### Editores de texto para MarkDown mas populares

* Escritorio (Windows, macOS, Linux) 
    * **Typora:** Interfaz limpia y minimalista, soporta tablas, diagramas, matemáticas (LaTeX) y exportación a múltiples formatos. Disponible para Windows, macOS y Linux.
    * **MarkText:**  Open Source y multiplataforma. Modo de vista previa en vivo y soporte para temas personalizados
    * **Obsidian:** Ideal para crear redes de conocimiento interconectadas. Soporte para plugins, gráficos y plantillas.
    * **Zettlr:** Manejo de referencias bibliográficas y citas con Zotero. Soporta matemáticas con LaTeX y exportación a PDF/Word/HTML.
    * **VS Code:** Extensiones como Markdown All in One y Markdown Preview Enhanced. Soporte para GitHub Flavored Markdown (GFM). 
* Basados en web
    * **Dillinger:**  Sin instalación, soporta exportación a HTML, PDF y Dropbox
    * **StackEdit:** Sincronización con Google Drive, OneDrive y GitHub
    * **HackMD:** Similar a Google Docs, pero con Markdown en tiempo real
* Apli**caciones móviles
    * **Joplin:** Multiplataforma y permite sincronización con Nextcloud, Dropbox o OneDrive. Disponible para Windows, macOS, Linux, Android e iOS
    * **iA Writer:** Disponible para Windows, macOS, iOS y Android.

### Buenas prácticas en MarkDown

* Organización y estructura del documento.
* Uso de comentarios ocultos en Markdown.
* Accesibilidad y compatibilidad entre diferentes plataformas.

--- 

## **Sintaxis de MarkDown**

### Encabezados

# Esto es un encabezado de nivel 1 (hay 6)
## Esto es un encabezado de nivel 2
### Esto es un encabezado de nivel 3
#### Esto es un encabezado de nivel 4
##### Esto es un encabezado de nivel 5
###### Esto es un encabezado de nivel 6

(Se necesita dejar un espacio entre los gatos y el encabezado)

---
### Párrafos 

Esto es un párrafo común y corriente. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

--- 

### Estilos de palabras 

Palabra en _cursiva_

Palabra en **negrita**

**_Cursiva y negrita_**

***cursiva y negrita***

___cursiva y negrita___

Palabra ~~tachada~~

Palabra ==resaltada==

---

### Enlaces

Se definen con unos corchetes donde ira el texto a mostrar y en seguida unos parentesis donde va el link, si queremos usar una ancla interna, en el parentesis va el simbolo de # seguido de la ancla, si esta ancla tiene varias palabras, usamos guion medio en vez del espacio

Nota: El funcionamiento y sintaxis de anclas dependerá del editor de texto

[Instagram](https://www.instagram.com/ing_manuelrs/)

[Ir a Encabezado 1](#esto-es-un-encabezado-de-nivel-1-hay-6)

También podemos hacer una lista de enlaces y mostrar texto en su hover de la siguiente manera

[Enlace 1][1], [Enlace 2][2], [Enlace 3][3]

[1]: http://google.com/
[2]: http://facebook.com/ "Ir a facebook"
[3]: http://x.com/

O como un enlace muy sencillo solo encerramos la url en los símbolos menor y mayor que

<http://google.com>

---

### Imágenes

Parecido a los enlaces, para las imagenes necesitamos un signos de exclamacion, despues un juego de corchetes y en seguida un par de parentesis, en los corchetes va el nombre que le querramos dar a la imagen (alt) y en los parentesis la ruta de la imagen, ya sea local o externa

Nota: Tambien podemos hacer listas de imagenes como lo hacemos con los enlaces

![Logo de vscode](https://chris-ayers.com/assets/images/vscode-logo.png)

Para redimensionar la imagen, despues del nombre de imagen ponemos | y el numero en pixeles (Esto depende del interprete)

![Manuel Instagram Perfil|100](https://upload.wikimedia.org/wikipedia/commons/thumb/9/99/Unofficial_JavaScript_logo_2.svg/640px-Unofficial_JavaScript_logo_2.svg.png)

--- 

### Divisiones

Las divisiones son lineas horizontales que nos ayudan a separar contenido, estas las declaramos por tres guiones medios

Antes de la division

---

Despues de la division

--- 

### Listas

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

También podemos hacer listas de tareas con guion medio y corchetes con un espacio dentro, para dejar una seleccionada ponemos una x dentro de los corchetes (Esto depende del interprete)
- [ ] tarea 1
- [ ] tarea 2
- [x] tarea 3

---

### Citas

Para hacer citas hacemos uso del símbolo mayor que, esto para una cita de línea

> Extraño al barrio pero mis sueños están fuera de el. - Manuel R.S.

Para hacer citas de bloque usamos el símbolo mayor que en todas las líneas usadas

> Hay tres cosas que no se pueden ocultar,
>
> el sol, la luna y la verdad.
>
> Teen golf

---

## Tablas

Para hacer tablas hacemos uso del símbolo pipe "|" como bordes verticales de nuestra tabla y después de los títulos usamos | acompañado de tres guiones medios por cada celda
Nota: No es necesario alinear las celdas y su contenido para que en modo edición parezca una tabla, markdown la interpreta si esta o no alineada

| Nombre    | Edad | Correo              |
| --------- | ---- | ------------------- |
| Manuel    | 21   | manuel@gmail.com    |
| Alejandro | 20   | alejandro@gmail.com |

Se puede especificar la alineación de cada columna mediante la adición de dos puntos a las líneas de separación. Dos puntos a la izquierda de la línea de separación hará que la columna esté alineada a la izquierda, dos puntos a la derecha de la línea hará que la columna esté alineada a la derecha, dos puntos en ambos lados significa que la columna se alinea al centro.

| Elemento | Cantidad | Precio |
| :------- | :------: | -----: |
| Item 1   | 15       | 150€   |
| Item 2   | 3250     | 23,65€ |

---

### Códigos

Para código en línea usamos acentos graves

La siguiente palabra `let` la usamos para definir una variable con scope local en js

Para código en bloque usamos tres acentos graves al inicio y al final del bloque de código, podemos especificar el lenguaje usado poniendo el nombre del lenguaje de programación usado en el bloque después de los primeros acentos

```javascript
const saludar = nombre => {
    console.log(`Hola ${nombre}`);
}
```

---

### Etiquetas HTML

Podemos escribir etiquetas HTML en markdown

<form>
    <label for="name">Nombre</label>
    <input type="text" id="name" placeholder="Escribe tu nombre..."></input>
</form>

---

### Comentarios

Para hacer un comentario en markdown es de la misma manera que en HTML o con dos simbolos de porcentaje al inicio y al final del comentario (este ultimo puede variar dependiendo del interprete)

<!-- Esto es un comentario -->
%% Esto es un comentario %%

---

### Ignorar sintaxis de markdown

Para ignorar caracteres que forman una sintaxis en markdown anteponemos una diagonal invertida en cada uno de estos caracteres

Palabra en \*\*negrita\*\*

---

### Sintaxis de anclas en Obsidian

Para usar anclas usamos dos corchetes anidados 

Para dirigirnos a una ancla en el mismo archivo: 

[[curso-md#Esto es un encabezado de nivel 1 (hay 6)]]

Podemos asignarle un label 

[[curso-md#Esto es un encabezado de nivel 1 (hay 6) | Encabezado 1]]

Crear un enlace a otro archivo 

[[otro-archivo | Ir a Otro archivo]]

Ir a una ancla de otro archivo 

[[otro-archivo#Titulo| Ir a Otro archivo]]
