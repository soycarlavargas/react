# Ecosistema de React #
Al momento de trabajar dentro de una aplicación React es muy común confundirnos y pensar que con esta librería vamos a poder construir absolutamente todo lo que habíamos hecho con anterioridad. La verdad es que esta línea de pensamiento está bastante alejada de la realidad.

Si bien React nos provee de todo un set de archivos e incluso bibliotecas de Node.js, al final del día todo lo que hacemos aquí solamente forma parte del frontend.

Pero entonces, ¿por qué al momento de crear la aplicación tenemos tantos archivos? ¿Cuáles son los más importantes? ¿A cuáles deberíamos prestar particular atención?
***
Llamamos __ecosistema__ al conjunto de herramientas adicionales, aplicaciones y librerías que permiten a __React__ trabajar como un framework.
Dentro del ecosistema de archivos de React, se ejecutan **dos librerias** muy importantes que permiten por un lado **empaquetar** todos los archivos de js en un solo archivo que pueda ser ejecutado por el navegador, y por otro, **traducir** cuaquier sentencia de js muy novedosa, a sentencia de js un poco más antigua pero que siga siendo más estable y 100% interpretada por todos los navegadores.
***
## Sistema de empaquetado ##
Para React, lograr que de todos los archivos con los que trabaja se pueda generar uno solo, es necesario que se ejecute por detras una libreria que recibe el nombre de ***WEBPACK*** (empaquetador de módulos). Esta libreria permite automatizar procesos de empaquetamiento donde se compilan muchos archivos de JS en uno solo. Logrando de esta forma que React, con esta libreria, resuelva uno de los dos temas: **la transmision de multiples archivos de JS a la app**. Gracias a ella podemos tener la seguridad que al navegador le va a llegar un solo archivo todo empaquetado.
***
## Un traductor de archivos ##
Qué pasa con aquellas sentencias del lenguaje que son demasiado nuevas y que algunos navegadores no pueden interpretar. Para ello React usa **BABEL**, libreria que cumple con la funcion de la **transpilacion**, el cual es un proceso de traduccion. Lo que sucede en este tipo de ruutina es que se toma un codigo que es demasiado nuevo, y se traduce su equivalente en un codigo estable interpretable por los navegadores.  
  
  ***Todo esto viene configurado para que no nos preocupemos por el tema***
