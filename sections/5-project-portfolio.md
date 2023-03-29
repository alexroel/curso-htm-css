# Proyecto de PORTAFOLIO





---
## Presentación del proyecto 


---
## Agregando estilos
El siguiente código es una serie de reglas de estilo CSS que se aplican a todos los elementos (*) en una página web y al elemento HTML en particular.

Aquí hay una explicación de cada una de las reglas:
~~~css
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    scroll-behavior: smooth;
    font-family: 'Open Sans', sans-serif;
    font-style: italic;
}
~~~

- `margin: 0`: establece el margen exterior de todos los elementos en la página a cero.
- `padding: 0`: establece el relleno interno de todos los elementos en la página a cero.
- `box-sizing: border-box`: asegura que el ancho y alto de un elemento incluya tanto el contenido como el borde y el relleno.
- `text-decoration: none`: elimina cualquier subrayado o decoración de texto predeterminado de los enlaces.
- `border: none`: elimina cualquier borde predeterminado que tenga un elemento.
- `outline: none`: elimina cualquier borde de contorno que tenga un elemento, lo que es especialmente útil para eliminar el contorno en los elementos cuando se hace clic en ellos.
- `scroll-behavior`: smooth: agrega un desplazamiento suave a los enlaces internos de la página.
- `font-family: 'Open Sans', sans-serif;`: establece la fuente predeterminada para la página como Open Sans, una fuente de tipo sans-serif, lo que significa que los caracteres no tienen serifs (pequeñas líneas o trazos en los bordes de las letras).
- `font-style: italic;`: establece el estilo de fuente predeterminado como cursiva o inclinado.
~~~css
html{
    font-size: 62%;
    overflow-x: hidden;
}
~~~

- `font-size: 62%;`: establece el tamaño de fuente predeterminado para el elemento HTML en un 62% del tamaño de fuente original, lo que puede ayudar a hacer que el texto en la página sea más legible en dispositivos móviles o pantallas de menor resolución.
- `overflow-x: hidden;`: oculta cualquier desplazamiento horizontal que pueda estar presente en la página, lo que puede mejorar la apariencia y la funcionalidad de la página.

~~~css
section {
    min-height: 100vh;
    padding: 10rem 9% 2rem;
}
~~~

- `min-height: 100vh;`: establece la altura mínima del elemento de sección al 100% del alto de la ventana gráfica (vh significa "viewport height"). Esta regla asegura que la sección se extienda por lo menos hasta la altura de la ventana gráfica, lo que significa que no habrá espacios en blanco en la parte inferior de la sección, incluso si el contenido es menor que la altura de la ventana gráfica.

- `padding: 10rem 9% 2rem;`: establece los valores de relleno (padding) para la sección. Los valores de relleno se especifican en el orden superior, derecho, inferior y izquierdo (en sentido horario, comenzando desde la parte superior). En este caso, la sección tiene un relleno superior e inferior de 10 "unidades" de la unidad de medida rem (que significa "tamaño de fuente raíz"), un relleno derecho e izquierdo del 9% del ancho del elemento y un relleno inferior de 2 "unidades" de rem. Estos valores de relleno permiten crear un espacio en blanco alrededor del contenido de la sección, lo que puede mejorar su legibilidad y su apariencia visual.

---
## Variables en CSS
En CSS, las variables se utilizan para almacenar valores y hacer que el código sea más fácil de mantener. Las variables se definen utilizando la sintaxis `--nombre-variable: valor;`. Por ejemplo:

~~~css
:root {
    --bg-color: #17202A;
    --second-bg-color: #1B2631;
    --text-color: #fff;
    --main-color: #1ABC9C;
}
~~~

En este ejemplo, se definen dos variables: `--bg-color` y `--second-bg-color`. Estas variables pueden ser utilizadas en cualquier parte del código CSS. Por ejemplo:

~~~css
body{
    background: var(--bg-color);
    color: var(--text-color);
}
~~~

En este ejemplo, se utilizan las variables definidas anteriormente para establecer el color de fondo, el color del borde y el color del texto de un botón, así como el color del texto de un enlace. Al utilizar variables, se hace que el código sea más fácil de mantener, ya que si se necesita cambiar el color primario o secundario, solo se necesita cambiar el valor de la variable, en lugar de cambiar manualmente cada lugar donde se utilizan esos colores.

Es importante destacar que las variables CSS pueden ser utilizadas en cualquier lugar donde se utilice una propiedad que acepte un valor. Las variables también pueden ser anidadas, lo que significa que una variable puede hacer referencia a otra variable.

---
## Encabezado
El siguiente código es una estructura HTML que representa el encabezado (`header`) de una página web. La estructura se compone de dos elementos principales: un logotipo (h1 con la clase logo) y un menú de navegación (nav con la clase navbar). El encabezado se ve así:

~~~html
    <!-- ESTRUCTURA DE HEADER
    =========================================== -->
    <header class="header">
        <h1 class="logo">Alex Roel</h1>

        <nav class="navbar">
            <a href="#inicio">Inicio</a>
            <a href="#habilidades">Habilidades</a>
            <a href="#proyectos">Proyectos</a>
            <a href="#testimonio">Testimonio</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>
~~~

El código es una regla de CSS que define un conjunto de propiedades de estilo para los elementos que tienen la clase `.header`. En concreto, las propiedades que se están definiendo son:

~~~css
.header {
    position:  fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 2rem 9%;
    background: var(--bg-color);
    display: flex;
    justify-content: space-between;
    align-items: certer;
    z-index: 100;
}
~~~

- `position: fixed;`: esta regla establece que el elemento .header debe tener una posición fija en la ventana del navegador, de modo que permanezca visible en la parte superior de la pantalla mientras el usuario desplaza el contenido de la página.

- `top: 0; left: 0; width: 100%;`: estas reglas establecen que el elemento .header debe colocarse en la esquina superior izquierda de la ventana del navegador y ocupar todo el ancho disponible (100% del ancho de la ventana).

- `padding: 2rem 9%;`: esta regla establece un relleno de 2 unidades de medida de altura y 9% de ancho en la parte superior e inferior y en los lados izquierdo y derecho del elemento .header, respectivamente.

- `background: var(--bg-color);`: esta regla establece un color de fondo para el elemento .header. En este caso, se está utilizando una variable CSS definida en otro lugar del código.

- `display: flex;`: esta regla establece que el elemento .header debe ser un contenedor flexible, lo que permite organizar el contenido dentro de él en filas o columnas.

- `justify-content: space-between;`: esta regla establece que el contenido dentro del elemento .header debe distribuirse de manera uniforme a lo largo del eje principal (horizontal), con un espacio adicional entre los elementos.

- `align-items: center;`: esta regla establece que el contenido dentro del elemento .header debe alinearse en el centro del eje secundario (vertical).

- `z-index: 100;`: esta regla establece la propiedad z-index del elemento .header, que determina la prioridad de su posición en la pila de elementos. En este caso, se establece un valor de 100, lo que significa que el elemento .header estará en un nivel superior a otros elementos de la página que tengan un valor z-index inferior.

~~~css
.logo{
    font-size: 2.5rem;
    color: var(--text-color);
    font-weight: 600;
    cursor: default;
}
~~~

Estas reglas de estilo CSS definen la apariencia del texto dentro del elemento .logo, incluyendo su tamaño, color, grosor de fuente y comportamiento del cursor.

~~~css
.navbar a{
    font-size: 1.7rem;
    color: var(--text-color);
    margin-left: 4rem;
    font-weight: 500;
}
~~~
Estas reglas de estilo CSS definen la apariencia de los enlaces dentro del elemento .navbar, incluyendo su tamaño, color, margen izquierdo y grosor de fuente.

---
## Seudo clases y elementos
En CSS, las pseudo-clases y pseudo-elementos son palabras clave que se usan para seleccionar elementos HTML en función de su estado o posición en el documento. Estas pseudo-clases y pseudo-elementos se agregan a un selector y se escriben después del selector principal separados por dos puntos (:).

A continuación, se explican las diferencias entre las pseudo-clases y pseudo-elementos:

- Pseudo-clases: Las pseudo-clases se usan para seleccionar elementos en función de su estado o interacción del usuario. Por ejemplo, :hover selecciona un elemento cuando el cursor del mouse se coloca sobre él, :active selecciona un elemento cuando está siendo activamente seleccionado por el usuario, :visited selecciona un enlace que ya ha sido visitado, entre otros.

- Pseudo-elementos: Los pseudo-elementos se usan para agregar elementos HTML virtuales a un documento. Por ejemplo, ::before y ::after permiten agregar contenido antes o después del contenido real de un elemento, ::first-letter y ::first-line permiten aplicar estilos específicos al primer carácter o línea de un elemento, entre otros.

A continuación se presentan algunos ejemplos de pseudo-clases y pseudo-elementos en CSS:

**Pseudo-clases:**

~~~css
/* Cambiar el color de un enlace al pasar el cursor por encima */
a:hover {
  color: red;
}

/* Cambiar el estilo de un enlace que se ha visitado */
a:visited {
  text-decoration: underline;
}

/* Cambiar el estilo de un enlace que está siendo activamente seleccionado */
a:active {
  background-color: yellow;
}
~~~

**Pseudo-elementos:**

~~~css
/* Agregar contenido antes de un elemento */
p::before {
  content: "Antes de este párrafo: ";
}

/* Agregar contenido después de un elemento */
p::after {
  content: "Después de este párrafo.";
}

/* Aplicar estilos a la primera letra de un párrafo */
p::first-letter {
  font-size: 2rem;
  font-weight: bold;
  color: red;
}
~~~

Es importante tener en cuenta que algunos navegadores antiguos pueden no admitir todas las pseudo-clases y pseudo-elementos. Por lo tanto, es recomendable comprobar la compatibilidad del navegador antes de usarlos en un proyecto.

~~~css
.navbar a:hover{
    color: var(--main-color);
}
~~~

---
## Sección de bienvenida
El elemento `main` es un elemento HTML5 que se utiliza para definir el contenido principal de una página. Dentro del elemento `main` se suele incluir todo el contenido relevante de la página, como los encabezados, el contenido de la página, el pie de página y otras secciones principales.

El elemento main contiene una sección de presentación (section.home) que incluye información sobre el autor, sus habilidades y enlaces a sus perfiles en redes sociales. También incluye una imagen del autor.
~~~html
    <main>
        <!-- ESTRUCTURA DE INICIO O PRESENTACIÓN
        =========================================== -->
        <section class="home" id="home">
            <div class="home-content">
                <h3>Hola, Yo soy</h3>
                <h1>Alex Roel</h1>
                <h3>Y Soy un <span>Desarrollador Web</span> </h3>
                <p>
                    Soy un desarrollador web especializado en crear sitios web atractivos, funcionales y seguros. Con habilidades en HTML, CSS, JavaScript y frameworks, me aseguro de que los sitios sean compatibles con diferentes navegadores y dispositivos móviles, y cumplan con los estándares de accesibilidad y usabilidad.
                </p>

                <div class="social-media">
                    <a href=""><i class='bx bxl-facebook'></i></a>
                    <a href=""><i class='bx bxl-youtube'></i></a>
                    <a href=""><i class='bx bxl-github'></i></a>
                    <a href=""><i class='bx bxl-linkedin'></i></a>
                </div>

                <a href="" class="btn">Descargar CV</a>
            </div>
            <div class="home-img">
                <img src="img/alexroel.png" alt="">
            </div>
        </section>

        ...
    </main>
~~~

~~~css
.home{
    display: flex;
    justify-content: center;
    align-items: center;
}

.home-content h3{
    font-size: 3.2rem;
    font-weight: 700;
}

.home-content h3:nth-of-type(2){
    margin-bottom: 2rem;
}
~~~

`.home-content h3:nth-of-type(2)` es un selector CSS que selecciona el segundo elemento h3 dentro del elemento con la clase home-content.

La pseudo-clase `:nth-of-type()` selecciona elementos que coinciden con un número ordinal específico en relación con el mismo tipo de elemento. En este caso, `:nth-of-type(2) `selecciona el segundo elemento h3.

margin-bottom es una propiedad CSS que define la cantidad de espacio en blanco que se agregará en la parte inferior de un elemento. En este caso, margin-bottom: 2rem establece un margen inferior de 2 unidades de medida rem para el segundo elemento h3 dentro de .home-content. Esto agrega un espacio en blanco adicional debajo del segundo encabezado h3.

~~~css
span{
    color: var(--main-color);
}
.home-content h1{
    font-size: 5.6rem;
    font-weight: 700;
    line-height: 1.3;
}

.home-content p{
    font-size: 1.7rem;
    font-weight: 400;
}

.home-img img{
    width: 30vw;
    border-radius: 5%;
    border: 5px solid #1ABC9C;
}
~~~

---
## Transiciones 
Las transiciones en CSS permiten animar un cambio de estado en un elemento, como un cambio en el color, tamaño o posición de un elemento, de una forma suave y gradual en lugar de brusca.

Para crear una transición, se especifican dos estados de un elemento y las propiedades que deben cambiar cuando se produce la transición. Por ejemplo:

~~~css
.btn {
  background-color: blue;
  transition: background-color 0.5s ease;
}

.btn:hover {
  background-color: red;
}
~~~

En este ejemplo, el botón tiene un color de fondo inicial azul y cuando se hace hover sobre él, el color de fondo cambia suavemente a rojo durante medio segundo (0.5s) con una transición de "ease".

La propiedad transition especifica qué propiedad CSS se va a animar y en qué cantidad de tiempo y velocidad se realizará la transición. El primer valor en la propiedad transition es la propiedad a animar (en este caso background-color) y el segundo valor es la duración de la transición (0.5s en este ejemplo). El tercer valor, ease, indica el tipo de curva de aceleración de la transición.

Hay varios tipos de curvas de aceleración (como ease, linear, ease-in, ease-out, ease-in-out, entre otros) que pueden ser utilizadas para personalizar la transición según tus necesidades.

~~~css
.social-media a{
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background: transparent;
    border: .2rem solid var(--main-color);
    border-radius: 50%;
    font-size: 2rem;
    color: var(--main-color);
    margin: 3rem 1.5rem 3rem 0;
    transition: .6s ease;
}

.social-media a:hover{
    background: var(--main-color);
    color: var(--second-bg-color);
    box-shadow: 0 0 1rem var(--main-color);
}


.btn{
    display: inline-block;
    padding: 1rem 2.8rem;
    background: var(--main-color);
    border-radius: 4rem;
    box-shadow: 0 0 1rem var(--main-color);
    font-size: 1.6rem;
    color: var(--second-bg-color);
    letter-spacing: .1rem;
    font-weight: 600;
    transition: .5s ease;
}

.btn:hover{
    box-shadow: none;
}
~~~

El código `box-shadow: 0 0 1rem var(--main-color);` es una propiedad CSS que se utiliza para aplicar sombras a un elemento en la página web.

La propiedad box-shadow acepta varios valores separados por espacios que definen las características de la sombra. En este caso, los valores son:

- 0 para la posición horizontal de la sombra.
- 0 para la posición vertical de la sombra.
- 1rem para el tamaño o difuminado de la sombra.
- var(--main-color) para el color de la sombra.

Por lo tanto, la sombra será de un tamaño de 1rem y tendrá el mismo color que la variable --main-color definida en la hoja de estilos CSS. La sombra se ubicará justo detrás del elemento, en la misma posición del elemento y se difuminará hacia afuera.

---
## Sección de about
El código que se muestra es una estructura HTML de una sección llamada "Acerca de" o "About" en inglés. Esta sección se utiliza comúnmente en páginas web para proporcionar información sobre el propietario o el equipo de una empresa o sitio web, y a menudo incluye una breve biografía, habilidades, experiencia y logros relevantes. La sección consta de dos partes: una imagen y un contenido de texto. En la parte de la imagen, se muestra la foto del desarrollador web, y en la parte de texto, se proporciona información sobre sus habilidades y experiencia en el desarrollo web. Además, hay un botón "Leer más" que podría ser utilizado para dirigir al usuario a otra página con más información sobre el desarrollador web.

~~~html
        <!-- ESTRUCTURA DE ABOUT O ACERCA DE 
        =========================================== -->
        <section class="about" id="about">
            <div class="about-img">
                <img src="img/alexroel.png" alt="">
            </div>
            <div class="about-content">
                <h2 class="heading">Acerca de <span>Mí</span></h2>
                <h3>Desarrollador web</h3>
                <p>
                    Alex Roel es un experimentado desarrollador web con más de 7 años de experiencia en la creación de
                    sitios web y aplicaciones. Con habilidades en lenguajes como HTML, CSS, JavaScript, y frameworks como
                    React, Vue, Angular, ha trabajado en una variedad de proyectos para clientes de diferentes industrias.
                    Su enfoque en la usabilidad y la accesibilidad, así como su capacidad para trabajar en equipo y cumplir
                    plazos, lo hacen un profesional confiable y exitoso en su campo.
                </p>
                <a href="" class="btn">Leer Más</a>
            </div>
        </section>
~~~

Este es un bloque de código CSS que establece los estilos para una clase llamada ".about". Aquí se detallan las propiedades que se aplicarán al elemento HTML que tiene la clase "about".

- La propiedad "display: flex" indica que los elementos hijos de este elemento se organizarán en una disposición flexbox, lo que significa que se pueden distribuir y alinear fácilmente en una dirección horizontal o vertical.

- La propiedad "justify-content: center" alinea los elementos hijos horizontalmente en el centro del contenedor "about".

- La propiedad "align-items: center" alinea los elementos hijos verticalmente en el centro del contenedor "about".

- La propiedad "gap: 2rem" establece un espacio de 2 unidades de medida "rem" entre los elementos hijos de la clase ".about".

- La propiedad "background: var(--second-bg-color)" establece el color de fondo de la clase ".about" utilizando una variable CSS que se ha definido en otra parte del código.

En resumen, estas propiedades trabajan juntas para crear un contenedor flexbox centrado vertical y horizontalmente, con un espacio uniforme entre sus elementos hijos y un fondo de color especificado.

~~~css
/* MAIN - SECCIÓN DE ABOUT O ACERCA DE 
===============================================*/
.about{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 2rem;
    background: var(--second-bg-color);
}

.about-img img{
    width: 30vw;
    border-radius: 5%;
    border: 5px solid #1ABC9C;
}

.heading{
    text-align: center;
    font-size: 4.5rem;
}

.about-content h2{
    text-align: left;
    line-height: 1.2;
}

.about-content h3{
    font-size: 2.6rem;
}

.about-content p{
    font-size: 1.7rem;
    margin: 2rem 0 3rem; 
}
~~~

---
## Sección de servicios

Este es un bloque de código HTML que representa una sección de servicios. Aquí se crea una sección con la clase "services" y un identificador "id" de "services".

-El título de la sección se define con la etiqueta "h2" y la clase "heading", y se usa la etiqueta "span" para agregar la palabra "Servicios" en negrita.

- A continuación, se crea un contenedor con la clase "services-container" que contiene varios elementos con la clase "services-box".

- Cada elemento "services-box" contiene un icono y un título que describen el servicio, así como un párrafo que explica brevemente en qué consiste el servicio.

- Finalmente, se agrega un botón "Leer Más" que se puede utilizar para obtener más información sobre el servicio.

~~~html
        <!-- ESTRUCTURA DE SERVICES O SERVICIOS 
        =========================================== -->
        <section class="services" id="services">
            <h2 class="heading">Nuestros <span>Servicios</span></h2>
    
            <div class="services-container">
                <div class="services-box">
                    <i class='bx bx-code-alt'></i>
                    <h3>Desarrollo Web</h3>
                    <p>
                        Desarrollo web: creación de sitios y aplicaciones web usando tecnologías como HTML, CSS, JavaScript,
                        y frameworks para mejorar la experiencia del usuario.
                    </p>
                    <a href="" class="btn">Leer Más</a>
                </div>
    
                <div class="services-box">
                    <i class='bx bx-code-curly'></i>
                    <h3>Desarrollo Backend</h3>
                    <p>
                        Desarrollo backend: creación y mantenimiento del servidor, la base de datos y la lógica de negocio
                        detrás de una aplicación web o móvil.
                    </p>
                    <a href="" class="btn">Leer Más</a>
                </div>
    
                <div class="services-box">
                    <i class='bx bx-support'></i>
                    <h3>Cursos de programación</h3>
                    <p>
                        Cursos de programación: enseñanza de lenguajes de programación, frameworks y herramientas para crear
                        aplicaciones web, móviles y de escritorio.
                    </p>
                    <a href="" class="btn">Leer Más</a>
                </div>
                <div class="services-box">
                    <i class='bx bx-code-alt'></i>
                    <h3>Desarrollo Web</h3>
                    <p>
                        Desarrollo web: creación de sitios y aplicaciones web usando tecnologías como HTML, CSS, JavaScript,
                        y frameworks para mejorar la experiencia del usuario.
                    </p>
                    <a href="" class="btn">Leer Más</a>
                </div>
    
                <div class="services-box">
                    <i class='bx bx-code-curly'></i>
                    <h3>Desarrollo Backend</h3>
                    <p>
                        Desarrollo backend: creación y mantenimiento del servidor, la base de datos y la lógica de negocio
                        detrás de una aplicación web o móvil.
                    </p>
                    <a href="" class="btn">Leer Más</a>
                </div>
    
                <div class="services-box">
                    <i class='bx bx-support'></i>
                    <h3>Cursos de programación</h3>
                    <p>
                        Cursos de programación: enseñanza de lenguajes de programación, frameworks y herramientas para crear
                        aplicaciones web, móviles y de escritorio.
                    </p>
                    <a href="" class="btn">Leer Más</a>
                </div>
            </div>
        </section>
~~~
Este es un conjunto de reglas CSS que se aplican a la sección de servicios o "services" de un sitio web.
~~~css
/* MAIN - SECCIÓN DE SERVICES O SERVICIOS 
===============================================*/
.services h2{
    margin-bottom: 5rem;
}

.services-container{
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 2rem;
}

.services-container .services-box{
    flex: 1 1 30rem;
    background: var(--second-bg-color);
    padding: 3rem 2rem 4rem;
    border-radius: 2rem;
    text-align: center;
    border: .2rem solid var(--bg-color);
    transition: .5s ease;
}

.services-container .services-box:hover{
    border-color: var(--main-color);
    transform: scale(1.02);
}
.services-box i{
    font-size: 7rem;
    color: var(--main-color);
}

.services-box h3{
    font-size: 2.6rem;
}

.services-box p{
    font-size: 1.7rem;
    margin: 1rem 0 3rem;
}
~~~

- También hay una propiedad "flex-wrap: wrap" que indica que los elementos dentro del contenedor deben envolverse a una nueva línea si el espacio no es suficiente. 
- Además, la propiedad "align-items: stretch" hace que los elementos se estiren verticalmente para que se alineen.
- Cada elemento tiene una anchura flexible (con "flex: 1 1 30rem"), lo que significa que se expandirá o encogerá según sea necesario, pero nunca será más ancho que 30rem. 
- transform: scale(1.02); es una propiedad de CSS que escala el elemento afectado en un cierto factor de escala especificado. En este caso, el factor de escala especificado es 1.02, lo que significa que el elemento se escalará en un 2% adicional sobre su tamaño original.
---
## Sección de portafolio

---
## Sección de contacto 


---
## Sección footer