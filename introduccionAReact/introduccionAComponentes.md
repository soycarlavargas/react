# Introducción a componentes #
Quizás una de las palabras que más se escucha nombrar al momento de introducirse en el mundo de React es “componente”. Pero, **¿qué es un componente?**

Los **componentes** son piezas funcionales y fundamentales de la aplicación, ya que nos van a permitir separar las distintas partes que conforman la estructura de un sitio web en pequeñas piezas independientes y reutilizables. Están pensados para que trabajen de forma aislada, pero que hagan parte de un “todo”.

Técnicamente, los componentes son funciones nativas de JavaScript que se ejecutan cada vez que sea necesario. Como cualquier función, pueden estar atadas, o no, a una serie de argumentos que nos permiten que este bloque de código pueda ser reutilizable, estableciendo que genere partes de la interfaz de usuario con información realmente dinámica.
***
## Stateless ##
Se llaman componentes __stateless__ porque internamente implementan un __return__ con lógica sencilla que entrega una estructura __HTML__

![stateless](/Imagenes/stateless.png)

## Crear un componente ##
Para iniciar la creación de un componente, primero debemos importar React y asegurarnos de que estamos exportando el componente que vamos a queresr implementar.

![crear un componente](/Imagenes/crearuncomponente.png)

## Implementar un componente ##
Debemos crear un archivo con extensión __.js__ con el nombre de la función que llevará dentro. En este caso **/src/components/Navbar.js**

![implementar un componente](/Imagenes/implementaruncomponente.png)  