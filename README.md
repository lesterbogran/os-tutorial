os-tutorial
===========

¡Cómo crear un SO desde cero!

Siempre he querido aprender a hacer un SO desde cero. En la universidad me enseñaron
Cómo implementar funciones avanzadas (paginación, semáforos, gestión de memoria, etc.)
pero:

- Nunca pude comenzar desde mi propio sector de arranque
- La universidad es difícil, así que no recuerdo la mayor parte.
- Estoy harto de personas que piensan que leer un núcleo ya existente, aunque sea pequeño, es
Una buena idea para aprender sistemas operativos.

Inspirado en [este documento] (http://www.cs.bham.ac.uk/~exr/lectures/opsys/10_11/lectures/os-dev.pdf)
y el [wiki de OSDev] (http://wiki.osdev.org/), intentaré hacer READMEs cortos y paso a paso y
ejemplos de código para que cualquiera los siga. Honestamente, este tutorial es básicamente el primer documento pero
dividido en piezas más pequeñas y sin la teoría.

Actualizado: más fuentes: [el pequeño libro sobre el desarrollo del sistema operativo] (https://littleosbook.github.io),
[Tutoriales de desarrollo del kernel de JamesM] (https://web.archive.org/web/20160412174753/http://www.jamesmolloy.co.uk/tutorial_html/index.html)


Caracteristicas
--------

- Este curso es un tutorial de código dirigido a personas que se sienten cómodas con la informática de bajo nivel. Por ejemplo,
programadores que tienen curiosidad sobre cómo funciona un sistema operativo pero no tienen el tiempo o la fuerza de voluntad para comenzar a leer el kernel de Linux
de arriba hacia abajo.
- Hay poca teoría. Sí, esta es una característica. Google es tu profesor de teoría. Una vez que pasas la universidad,
La teoría excesiva es peor que ninguna teoría porque hace que las cosas parezcan más difíciles de lo que realmente son.
- Las lecciones son pequeñas y pueden tardar entre 5 y 15 minutos en completarse. Confía en mí y confía en ti mismo. ¡Puedes hacerlo!


Cómo usar este tutorial
------------------------

1. Comience con la primera carpeta y baje en orden. Se basan en el código anterior, así que si
saltas directamente a la carpeta 05 y no sabes por qué hay un `mov ah, 0x0e`, es porque te perdiste la clase 02.
Realmente, solo ve en orden. Siempre puedes saltear cosas que ya sabes.

2. Abra el archivo README y lea la primera línea, que detalla los conceptos con los que debe estar familiarizado
antes de leer el código. Conceptos de Google con los que no estás familiarizado. La segunda línea establece los objetivos para cada lección.
Léelos, porque explican por qué hacemos lo que hacemos. El "por qué" es tan importante como el "cómo".
 
3. Lea el resto del archivo README. Es ** muy conciso **.

4. (Opcional) Intente escribir los archivos de código usted mismo después de leer el archivo README.

5. Mira los ejemplos de código. Están extremadamente bien comentados.

6. (Opcional) Experimente con ellos e intente romper cosas. La única forma de asegurarse de que entendió algo es
tratando de romperlo o replicarlo con diferentes comandos.


TL; DR: Primero lea el archivo README en cada carpeta, luego los archivos de código. Si eres valiente, intenta codificarlos tú mismo.


Estrategia
--------

Queremos hacer muchas cosas con nuestro sistema operativo:

- Arranque desde cero, sin GRUB - ¡HECHO!
- Ingrese al modo de 32 bits - HECHO
- Salta de la Asamblea a C - ¡HECHO!
- Manejo de interrupciones - ¡HECHO!
- Salida de pantalla y entrada de teclado - ¡HECHO!
- Un pequeño 'libc' básico que crece para satisfacer nuestras necesidades - ¡HECHO!
- Gestión de la memoria
- Escribir un sistema de archivos para almacenar archivos
- Crea un caparazón muy simple
- Modo de usuario
- Tal vez escribiremos un editor de texto simple
- Múltiples procesos y programación

Probablemente los revisaremos en ese orden, sin embargo, es pronto para contarlo.

Si nos sentimos lo suficientemente valientes:

- ¡Un intérprete BÁSICO, como en los años 70!
- Una GUI
- Redes



Contribuyendo
------------

Este es un proyecto de aprendizaje personal, y aunque no se ha actualizado durante mucho tiempo, todavía tengo la esperanza de entrar en él en algún momento.

Estoy agradecido a todos aquellos que han señalado errores y enviado solicitudes de extracción. Necesitaré algo de tiempo para revisar todo y no puedo garantizarlo en este momento.

Por favor, siéntase libre de bifurcar este repositorio. Si muchos de ustedes están interesados ​​en continuar el proyecto, háganmelo saber y vincularé la "bifurcación principal" desde aquí.
