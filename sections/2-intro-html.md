# Introducción a HTML

1. [¿Qué es HTML?](#¿qué-es-html)
2. [Sintaxis y etiquetas](#sintaxis-y-etiquetas)
3. [Estructura básica de un documento HTML](#estructura-básica-de-un-documento-html)
4. [Mi primer página](#mi-primer-página) 
5. [Etiquetas de texto](#etiquetas-de-texto)
6. [Ejemplo sobre etiquetas de texto](#ejemplo-sobre-etiquetas-de-texto)
7. [Herramientas para desarrollar](#herramientas-para-desarrollar)

---
## ¿Qué es HTML?
HTML significa "HyperText Markup Language" (Lenguaje de Marcado de Hipertexto), y es el lenguaje utilizado para crear y estructurar el contenido de las páginas web.

En términos más simples, HTML es un conjunto de etiquetas (o "marcas") que se utilizan para describir el contenido de una página web. Las etiquetas se utilizan para definir los elementos como títulos, párrafos, enlaces, imágenes, listas, formularios, entre otros.

HTML es el lenguaje básico de la web y es interpretado por los navegadores web. Cuando creas una página web en HTML, tu navegador interpreta el código HTML y muestra el contenido en pantalla.

El HTML se ha ido actualizando a lo largo de los años, con la última versión siendo HTML5. HTML5 ha introducido nuevas características y etiquetas que hacen más fácil crear sitios web modernos y eficientes.

---
## Sintaxis y etiquetas

La sintaxis de HTML consiste en etiquetas que se utilizan para crear elementos. Una etiqueta HTML consta de un nombre de etiqueta rodeado de corchetes angulares `< >`. 

Los elementos pueden tener atributos que se utilizan para proporcionar información adicional sobre el elemento. Los atributos se agregan a la etiqueta de apertura del elemento y constan de un nombre y un valor, separados por un signo igual. 

La mayoría de los elementos de HTML tienen una etiqueta de apertura y una etiqueta de cierre, que se utilizan para indicar el comienzo y el final del elemento. El contenido del elemento se coloca entre las etiquetas de apertura y cierre.

Aquí hay algunos ejemplos de etiquetas HTML comunes:

- `<html>`: Define el inicio del documento HTML.
- `<head>`: Define la sección de encabezado del documento.
- `<title>`: Define el título del documento, que aparece en la pestaña del navegador.
- `<body>`: Define la sección principal del documento, que contiene todo el contenido visible.
`<h1>` a `<h6>`: Define encabezados con diferentes niveles de importancia.
`<p>`: Define un párrafo de texto.
`<img>`: Inserta una imagen en el documento.
`<a>`: Define un enlace a otro documento o recurso web.

Además, hay etiquetas HTML que no tienen etiqueta de cierre, como `<br>` para salto de línea y `<hr>` para una línea horizontal. Estas etiquetas se denominan etiquetas de "autocierre".

### Partes de un elemento HTML

- **Etiqueta de apertura**: indica el inicio del elemento y el tipo de elemento que se está utilizando. Se escribe entre corchetes angulares `< >` y puede incluir atributos. Por ejemplo, `<p>` es la etiqueta de apertura para un párrafo.

- **Contenido**: es el texto o elementos que se encuentran dentro del elemento. Por ejemplo, el texto que se escribe dentro de la etiqueta de apertura y cierre de un párrafo `<p> `y `</p>`.

- **Etiqueta de cierre**: indica el final del elemento y se escribe entre corchetes angulares, con una barra diagonal antes del nombre del elemento. Por ejemplo, `</p>` es la etiqueta de cierre para un párrafo.

- **Atributos**: proporcionan información adicional sobre el elemento y se utilizan para personalizar el comportamiento o la apariencia del elemento. Se escriben dentro de la etiqueta de apertura y consisten en un nombre y un valor, separados por un signo igual. Por ejemplo, el atributo `src` se utiliza para especificar la URL de una imagen en un elemento `<img>`.

#### Ejemplos de un elemento HTML
Aquí hay un ejemplo de un elemento HTML que muestra un párrafo:

~~~html
<p>Este es un párrafo de ejemplo.</p>
~~~

- **Etiqueta de apertura**: `<p>`
- **Contenido**: "Este es un párrafo de ejemplo."
- **Etiqueta de cierre**: </p>

Aquí hay un ejemplo de un elemento que muestra una imagen con atributos. 

~~~html
<img src="roelcode.png" alt="Logo de roelcode">
~~~

- **Atributos**: `src` con valor "`roelcode.png`" y `alt` con valor "`Logo de roelcode`".
Es importante tener en cuenta que no todos los elementos HTML tienen contenido o atributos, pero la mayoria ellos tienen etiquetas de apertura y cierre.

---
## Estructura básica de un documento HTML
La estructura básica de un documento HTML consta de dos partes principales: el encabezado (head) y el cuerpo (body). Aquí hay un ejemplo de la estructura básica de un documento HTML:

~~~html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi página</title>
</head>
<body>
    <!-- Contenido de la página -->
    <h1>Hola Mundo</h1>
    <p>Este es mi primer párrafo de ejemplo.</p>
</body>
</html>
~~~

El código HTML proporcionado es la estructura básica de una página web y consta de los siguientes elementos:

- `<!DOCTYPE html>`: Declaración de tipo de documento HTML, que indica que el documento es un archivo HTML5.

- `<html lang="es">`: Elemento raíz de la página, que indica que todo el contenido de la página se encuentra dentro de este elemento. También se especifica que el idioma predeterminado de la página es el español.

- `<head>`: Sección que contiene metadatos sobre la página y otros elementos que no se muestran en la página, como la información de la ventana del navegador.

- `<meta charset="UTF-8">`: Especifica el juego de caracteres utilizado en la página, que en este caso es UTF-8.

- `<meta http-equiv="X-UA-Compatible" content="IE=edge">`: Define el modo de compatibilidad de Internet Explorer, que en este caso se establece en el modo de compatibilidad más reciente.

- `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Define las dimensiones y la escala de la página en dispositivos móviles y tabletas.

- `<title>Mi página</title>`: Define el título de la página que aparece en la pestaña del navegador.

- `<body>`: Contiene todo el contenido visible de la página.

- `<h1>Hola Mundo</h1>`: Crea un encabezado de nivel 1 que dice "Hola Mundo".

- `<p>Este es mi primer párrafo de ejemplo.</p>`: Crea un párrafo que dice "Este es mi primer párrafo de ejemplo".

En resumen, este código define la estructura básica de una página web, establece el título de la página, define el idioma predeterminado y el conjunto de caracteres utilizado, así como el contenido visible de la página.

---
## Mi primer página
Aquí tienes una tarea para crear tu primera página web:

Objetivo: Crear una página web con un encabezado de bienvenida y un párrafo de presentación.

**Instrucciones**:

- Elije un tema para tu página web, puede ser algo relacionado con tus intereses, tu carrera, un proyecto escolar, etc.
- Crea un archivo HTML básico con las etiquetas necesarias para crear una página web. Asegúrate de incluir las etiquetas HTML, HEAD y BODY.
- En el encabezado (HEAD) de la página, incluye un título que describa el contenido de la página web. 
- En el cuerpo (BODY) de la página, agrega un encabezado de bienvenida que invite a los visitantes a conocer tu página. Puede ser algo como "Bienvenidos a mi página web sobre [tu tema]", o cualquier otro mensaje que prefieras.
- A continuación, escribe un párrafo de presentación en el que expliques el objetivo de tu página web y el contenido que los visitantes pueden encontrar.
- Revisa tu página web para asegurarte de que todas las etiquetas estén cerradas correctamente y de que el contenido se vea bien en diferentes dispositivos y navegadores.

~~~html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Web</title>
</head>

<body>
    <!-- Contenido de la página -->
    <h1>Bienvenidos a mi página</h1>
    <p>
        Mi nombre es Alex Roel y en este blog podrás encontrar todo tipo de contenido. Desde tutoriales sobre
        programación, hasta artículos de opinión sobre temas de actualidad.
    </p>

</body>

</html>
~~~
---
## Etiquetas de texto
Algunas etiquetas de texto en HTML incluyen:

- `<p>`: Define un párrafo de texto.
- `<h1>, <h2>, <h3>, <h4>, <h5>, <h6>`: Encabezados de distintos niveles, del 1 al 6.
- `<em>`: Emplea la cursiva para enfatizar una parte del texto.
- `<strong>`: Aplica negrita a una parte del texto para darle mayor importancia.
- `<sup>`: Coloca el texto en la parte superior de la línea, como en una exponente.
- `<sub>`: Coloca el texto en la parte inferior de la línea, como en una fórmula química.
- `<br>`: Inserta un salto de línea sin crear un nuevo párrafo.
- `<hr>`: Inserta una línea horizontal para separar distintas secciones de la página.
- `<pre>`: Se utiliza para mostrar texto formateado de una manera predefinida. 
- `<code>`: Se utiliza para resaltar el código dentro de un párrafo o una sección de texto, lo que hace que se vea diferente al texto normal y sea más fácil de identificar como código.

Estas etiquetas son solo algunas de las muchas que se pueden usar para dar formato y estilo al texto de una página web. Cada una tiene sus propios atributos y propiedades que se pueden utilizar para personalizar su apariencia.

---
## Ejemplo sobre etiquetas de texto
En este ejemplo utlilizaremos la mayoria de las etiquetas de texto. 

~~~html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi Web</title>
</head>

<body>

    <!-- Contenido de la página -->
    <h1>Bienvenidos a mi página</h1>
    <p>
        Mi nombre es Alex Roel y en este blog podrás encontrar todo tipo de contenido. Desde tutoriales sobre
        programación, hasta artículos de opinión sobre temas de actualidad.
    </p>

    <!-- Ejemplo 01 de etiquetas de texto -->
    <hr>
    <h2>Cálculo del área de un círculo</h2>

    <p>
        El área de un círculo se calcula multiplicando π (pi) por el radio al cuadrado. Mientras que el perímetro de un
        círculo, también conocido como circunferencia, se calcula multiplicando 2π (pi) por el radio.
    </p>

    <h3>Ejemplo</h3>

    <p>Supongamos que tenemos un círculo con un radio de 5 cm.</p>

    <h4>Cálculo del área</h4>
    <p>Para calcular el área, usamos la fórmula:</p>

    <pre>Área = π x r<sup>2</sup></pre>
    <p>Sustituyendo los valores, obtenemos:</p>
    <pre>a = 3.141592 x 5<sup>2</sup> = 78,5 cm<sup>2</sup></pre>

    <!-- Ejemplo 02 de etiquetas de texto -->
    <br>
    <hr>
    <h2>Fórmulas Químicas</h2>
    <p>
        En química, una fórmula química es una forma de expresar información acerca de las proporciones de los átomos
        que
        constituyen un compuesto químico. A continuación, se muestran algunas fórmulas comunes:
    </p>

    <h3>Agua</h3>
    <p>
        La fórmula química del agua es <strong>H<sub>2</sub>O</strong>. Esto significa que una molécula de agua está
        compuesta por dos átomos de hidrógeno y un átomo de oxígeno.
    </p>

    <!-- Ejemplo 03 de etiquetas de texto -->
    <hr>
    <h2>Hola mundo con HTML</h2>

    <p>
        Para imprimir "Hola mundo" en HTML se utiliza la etiqueta <b><code>h1</code> </b>, que es una etiqueta de
        encabezado de nivel 1. El siguiente código mostrará "Hola mundo" en el navegador:
    </p>

    <pre>
        <code>
            &lt;!DOCTYPE html&gt;
            &lt;html&gt;
                &lt;head&gt;
                    &lt;title&gt;Mi primera página en HTML&lt;/title&gt;
                &lt;/head&gt;
                &lt;body&gt;
                    &lt;h1&gt;Hola mundo&lt;/h1&gt;
                &lt;/body&gt;
            &lt;/html&gt;
        </code>
    </pre>

</body>

</html>
~~~

---
## Herramientas para desarrollar
Consola de desarrollador: Es una herramienta integrada en los navegadores web que permite depurar y analizar problemas en el código de una página web, visualizar y manipular el DOM, probar código JavaScript y realizar pruebas de rendimiento, entre otras funciones.






