# Práctica 9. Random Walk. Programación Gráfica y Orientada a Objetos en JS.
### Factor de ponderación: 8

### Objetivos

Los objetivos de esta práctica son:

* Poner en práctica metodologías y conceptos de Programación Orientada a Objetos.
* Practicar el proceso de pruebas de software (testing) utilizando Mocha y Chai.
* Practicar la evaluación del cubrimiento de código usando Istanbul.
* Poner en práctica la metodología de desarrollo TDD.

### Rúbrica de evaluacion del ejercicio
Se señalan a continuación los aspectos más relevantes (la lista no es exhaustiva)
que se tendrán en cuenta a la hora de evaluar este ejercicio:
* El comportamiento del programa debe ajustarse a lo solicitado en este enunciado.
* Deben usarse estructuras de datos adecuadas para representar los diferentes elementos que intervienen en el problema.
* Capacidad del programador(a) de introducir cambios en el programa desarrollado.
* Han de aportarse los tests utilizados para probar la aplicación en su fase de desarrollo.
* Han de aportarse los informes sobre cubrimiento de código de su aplicación.
* El programa debe ajustarse al paradigma de Orientación a Objetos.
* El formato del código ha de cumplir con lo establecido en la [Guía de Estilo de Google](https://google.github.io/styleguide/jsguide.html)
para Javascript. Utilice [ESLint](https://eslint.org/), convenientemente configurado, si se considera necesario para cumplir con este requisito.
* El código ha de estar documentado con [JSDoc](https://jsdoc.app/).
* Modularidad: el programa ha de escribirse de modo que las diferentes funcionalidades
que se precisen sean encapsuladas en módulos, clases, funciones y métodos cuya extensión léxica se
mantenga acotada.
* Eficiencia del código desarrollado.

### Presentación de resultados y ejecución de la aplicación
**Comience su trabajo** subiendo a la tarea correspondiente del aula virtual de la asignatura el enlace (git) a su repositorio privado de trabajo para esta práctica.

Toda la información que sigue:
* Ejecución de la aplicación (Enlace `Random Walk`)
* Documentación de la aplicación (enlace `Random Walk - Documentación`)
* Resultados de las pruebas desarrolladas (enlace `Random Walk - Tests`)
* Informe de cubrimiento de código (enlace `Random Walk - Cubrimiento`)
* Diagrama UML de la aplicación (enlace `Random Walk - UML`)
* Reserve asimismo en `index.html` un enlace adicional (`Ejercicio evaluación para el ejercicio que realizará
  durante la sesión de evaluación.

Se han de mostrar a través de una página `index.html` alojada en el servidor de su máquina IaaS de la asignatura. 
**Todas** las páginas que se muestran enlazadas a través de `index.html` han de tener como título (etiqueta
`title` de HTML) apellidos y nombre del autor de la aplicación. 
Asimismo apellidos y nombre deben figurar en las diferentes páginas indexadas (etiqueta `h1` de HTML).

Indexe en esa página principal cualquier resultado adicional que desee mostrar como evidencias para la evaluación de su trabajo.

El servidor web que aloja estas páginas ha de seguir funcionando después de cerrar la sesión en la máquina
IaaS-ULL que aloja el servidor para posibilitar la evaluación del trabajo realizado.

### Camino Aleatorio
El [camino aleatorio](https://en.wikipedia.org/wiki/Random_walk)
o paseo aleatorio, abreviado en inglés como RW (*Random Walks*), es una formalización matemática 
de la trayectoria que resulta de hacer sucesivos pasos aleatorios. 
Por ejemplo, la ruta trazada por una molécula mientras viaja por un líquido o un gas, el camino que sigue un animal en su 
búsqueda de comida, el precio de una acción fluctuante y la situación financiera de un jugador pueden tratarse como un camino aleatorio.


En el desarrollo de la aplicación que se propone, aplique el
[enfoque TDD](https://en.wikipedia.org/wiki/Test-driven_development) 
iterando las fases que se definen metodología:
Red - Green - Refactor - [Integrate] y escribiendo la documentación de la misma al mismo tiempo que desarrolla el código.

### Aplicación Random Walk
En esta práctica se propone desarrollar una aplicación JavaScript que muestre una camino aleatorio que comience en el centro de
un Canvas de forma rectangular que abarque la mayor parte del viewport del naveador y finalice cuando el
camino alcance cualquiera de los bordes del canvas.

El programa mostrará en el lienzo una cuadrícula con una determinada densidad (número de intersecciones).

La Figura \ref{fig} muestra ejemplos de caminos aleatorios dibujados sobre retículas de diferente densidad.

El camino aleatorio (como muestra la Figura \ref{fig}) se dibujará de modo que sólo recorre líneas de la cuadrícula 
(no se pueden trazar líneas de forma arbitraria en la ventana).

\subsection{Consideraciones} 
El programa se diseñará de tal modo que al ejecutarse, la retícula sobre la que se dibuja el camino ocupe 
toda (o la mayor parte) de la pantalla.

La aplicación estará preparada para dibujar en pantalla cuadrículas con alta densidad (digamos del orden de $100 \times 100$
puntos en la cuadrícula, o incluso superior).

Se deja libertad para cada uno de ustedes añada botones y/o controles adicionales a los propuestos, pero
la aplicación deberá al menos contemplar las especificaciones solicitadas en este documento.

### Ejercicios
