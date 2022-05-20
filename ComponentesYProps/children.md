# Children #
Seguramente van a existir casos en los que tengamos un componente tan dinámico que no conoceremos sus hijos de antemano. Esto es especialmente común para componentes como *Sidebar o Dialog* que representan cajas genéricas.

Es aquí donde cobra particular protagonismo la prop especial ***children***. A través de ella vamos a tener la capacidad de enviar cualquier tipo de estructura.

Por ejemplo, el siguiente componente *Saludo* renderizará el contenido de *props.children* dentro de un div:

![child1](/Imagenes/child1.png)

Esto nos permite que otros componentes les pasen hijos entre las etiquetas del componente, anidando el JSX en el rsultado final:

![child2](/Imagenes/child2.png) 
***

Para React, todo lo que sucede al momento de usar un componente, debe ser especificado cuando se crea el mismo. 
>"**Si el componente va a tener props y contenido entre sus etiquetas,** esto lo tenés que especificar"
***
Y es aquí donde entra el concepto de **Children** (hijos).
>Son todos aquellos elementos que son pasados entre sus etiquetas, **no como props si no como hijos del componente.**
***
Para preparar a un componente para recibir hijos, tenemos que hacer uso nuevamente de las **props**. Todo componente dentro de este gran objeto literal que son las props, tiene una propiedad particular llamada **CHILDREN**, la cual traerá consigo todos los elementos que se hayan dispuesto entre las etiquetas del componente, al momento en el que el mismo fue utilizado.  
Si pensamos en este componente:
![saludo](/Imagenes/saludo.png)
lo único que necesitamos hacer dentro de la función que define al componente, es esto: 
![child2](/Imagenes/child3.png)
De esta manera le estamos indicando al componente, que puede llegar a recibir hijos. Y si ese fuera el caso, se prepare para imprimirlos ahí, donde nosotros lo especificamos.
>IMPORTANTE! Sea que pasemos un solo children, o muchos, lo mismos se van a imprimir en ese orden exacto en el que fueron dispuestos al ser enviados, ya que todos se mandan en la misma prop.
***
Tener acceso a esta prop de un componente, hace que el mismo se convierta en algo **super poderoso**, ya que ahora no solo tenemos un conjunto de props que son dinamicas, sino que a su vez **el componente cuenta con la posibilidad de tener tantos hijos como creamos necesario.**
![child4](/Imagenes/child4.png)
![child5](/Imagenes/child5.png)
![child6](/Imagenes/child6.png)
Es importante corregir la mayuscula cuando importamos el componente, sino se rompe todo.
![childerror](/Imagenes/childerror.png)
### Resultados ###
![publi1](/Imagenes/publi1.png)
![publi2](/Imagenes/publi2.png)
En ambos tenemos cierta estructura en común, pero no sabemos bien qué nos va a venir dentro del componente.

## SLIDES ##
![schild1](/Imagenes/schild1.png)
![schild2](/Imagenes/schild2.png)
![schild3](/Imagenes/schild3.png)
![schild4](/Imagenes/schild4.png)