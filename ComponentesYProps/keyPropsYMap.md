# Keyprops #
Las usamos cuando no sabemos con exactitud qué cantidad de elementos va a terminar renderizando nuestro componente. Es donde se hace necesario trabajar con **arrays** y sus **métodos**. De esta forma ya no nos interesa si a nuestro componente le pasan 1, 2 o 15 enlaces, ya que los mismos van a ser pasados como un **array** a través de las **props**. Dentro del componente, nuestro trabajo será iterar sobre ese array e imprimir la cantidad de enlaces que corresponda.  
![keyprop](/Imagenes/keyprop.png)  
El **array** es pasado dentro del atributo con nombre **enlaces** y que adicionalmente va entre llaves **{}** porque son estas llaves las que te **permiten escribir tipos de datos de JS** que no sean simplemente cadenas de texto.  
Dentro del componente, lo primero que tenemos que hacer es recibir laas props como param de la funcion. Luego, dentro de la estructura de JSX que hayas definido, vas a tener que iterar sobre el array recibido para poder imprimir estos enlaces.  
# Map #
El método que debemos implementar es el método map. El mismo itera sobre cada uno de los elementos de ese array y retorna un resultado por cada uno de los elementos. Y es aqui, en este retorno, en donde el elemento podrá renderiarse perfectamente. Por esto, es que el componente se va a ver algo así:
![componente](/Imagenes/componente.png)  
Dentro de la lista tipo UL van un par de llaves y dentro de estas mismas se está haciendo referencia a la prop **enlaces** que recibe el componente, la cual es un array.  
Es sobre dicha propiedad que se ejecuta el método map *(map se ejecuta sobre un array)*. Dentro del map se está retornando **una estructura de JSX** que contiene al elemento li y entre las etiquetas li se está imprimiendo a cada enlace haciendo uso tmb de **las llaves** para poder mostrar el texto correspondiente. Es decir, el map nos va a retornar por cada uno de los elementos del array un bloque de JSX.
![NavBar](/Imagenes/navbar.png)  
Quedando algo así:
- Home
- Productos
- Servicios
- Sucursales
- Contacto
***
Los componentes que van a renderiazar varios elementos del mismo tipo (como en este caso que tenemos muchos li pero no sabemos cuantos), necesitan de una **key con valor unico**, porque la misma va a ayudar a react a identificar luego que items han cambiado, cuales han sido agregados, eliminados... Por esto las keys deben ser dadas a los elementos dentro del mapeo del array, para darle a los **elementos** una **identidad única y estable.**  
Para esto vamos a usar el atributo ***key*** al cual le daremos un valor único, algo más o menos así:
![NavBar](/Imagenes/navbar1.png)  
Ahora el elemento li tiene un atributo llamado key y al mismo se está asignando el valor corresp al texto de cada enlace, más el indice en el cual se encuentra el mismo dentro del array. Por lo tanto, cada key quedará armada de la siguiente manera:
- Home0
- Productos1
- Servicios2
- Sucursales3
- Contacto4  

Como vemos, cada elemento de tipo li, que se está renderizando, cuenta con un **identificador unico**, que lo hace diferente de sus demas elementos hermanos.  
___Esto es fundamental para que React trabaje perfectamente.___  
>Este atributo no es imprime realmente como un atributo HTML, es decir nunca lo vamos a ver en el navegador ni en la consola, porque ese dato es de uso exclusivo para React
***
![Ejercicio1](/Imagenes/ejercicio1.png)  
![Ejercicio2](/Imagenes/ejercicio2.png)  
![Ejercicio3](/Imagenes/ejercicio3.png)  
![Ejercicio4](/Imagenes/ejercicio4.png)  
___Como regla general, podemo4 saber que cada vez que ten4mos un array, ya 4ea recibido por props o en 4na variable, vamo4 a utilizar el map para hace un output para cada uno de los elementos. Y vamos a jugar con la posibilidad de tener un i en el map y el map, y el atributo key, para darle un atributo unico para que React funcione como está estipulado.___
***
## SLIDES ##
![map1](/Imagenes/slidemap1.png)  
![map2](/Imagenes/slidemap2.png)
![map3](/Imagenes/slidemap3.png)  
![keys1](/Imagenes/slidekeys1.png)
![keyprops1](/Imagenes/slidekeyprops1.png)  
![keyprops2](/Imagenes/slidekeyprops2.png)  