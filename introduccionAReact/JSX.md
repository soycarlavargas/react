# JSX / JavaScript XML #
Es una extensión de la sintaxis de JavaScript que sirve para generar bloques de código HTML, pero con sentencias de JavaScript.

En sí, JSX es muy parecido al HTML, pero con ciertas particularidades que lo hacen diferente. Este puede ser utilizado única y exclusivamente dentro del entorno de React.

Pero si se parece tanto a HTML, ¿por qué no usamos solo HTML?

React propone este formato ya que es consciente de que, al momento de generar la estructura interna de un componente, es muy seguro que mucho de ese código lo vamos a querer dinámico y reutilizable. Es aquí donde JSX cobra una vital importancia.

Para dar un ejemplo, un bloque sencillo de código en JSX se verá así:

![jsx](/Imagenes/jsx.png)

Como vemos, JSX no es tan distante de HTML, incluso se parece un poco a EJS.

Veamos entonces mucho más en detalle de qué trata esta nueva, pero sencilla, forma de escritura.
***
##  Interpolando datos ##
Declaramos una variable llamada __name__ y luego la usamos dentro del JSX __encerrándola__ dentro de llaves. _Se puede colocar cualquier expresión de JS dentro de llaves en JSX_

![jsx ejemplo](/Imagenes/jsxejemplo.png)
