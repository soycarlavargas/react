¿Qué pasaría si dentro de nuestro componente, en el lugar que esperamos recibir un array para iterarlo, recibimos un string? ¿El método **.map**() seguirá funcionando? ¿El componente se renderizará bien?

Para solucionar este problema existen las **PropTypes**. Con ellas podemos determinar específicamente el tipo de dato de una prop. React validará las props pasadas a un componente según las definiciones que hayamos establecido para esas props y levantará una advertencia en tiempo de desarrollo si algún criterio no se cumple.

**PropTypes** funciona como una biblioteca externa desde la versión 15.5 de React, por lo que, si queremos aprovechar sus ventajas, necesitamos instalar este paquete haciendo uso del siguiente comando:

       npm install prop-types --save  
          
Junto a **PropTypes**, existen las **DefaultProps** que nos permiten definir valores por defecto para determinadas props. Claramente, las personas que programaron React pensaron en todo.

# PropTypes #
>Es una manera en la que podés definir el tipo de dato que se espera recibir para una determinada prop de un componente.
***
Una vez que hayamos instalado el **prop-types**, tenemos que **importar** dicho paquete en el componente donde lo querramos usar.
>"no todos los componentes necesitan de estas ___propTypes___, son más que nada una ___ayuda___ a nivel escritura de código que nos va a permitir estar al tanto de posibles errores en el uso de nuestros componentes"  
***
  Con el paquete ya importado dentro del componente, tenemos que hacer algo así:  

        import propTypes from 'prop-types';  
          
Alcanza con definir que para ese componente, queremos hacer uso de las **prop-types**.  
Estamos dentro del componente **NavBar** y queremos definir el tipo de dato que la prop enlaces espera recibir.  
Para esto, dentro del mismo archivo del componente, y antes de la exportación del mismo, vamos a asignar al componente, una propiedad llamada **propTypes**, a la cual le vamos a asignar como valor un **objeto literal**.  
_Dentro de este objeto literal_, vamos a tener que hacer referencia al **nombre de la prop** a la cual le queremos especificar el tipo de dato y a ella le vamos a asignar, usando el paquete  **prop types:**

![navbarpt](/Imagenes/navbarpt.png)  
>OBSERVEMOS como la propiedad asignada al nombre del componente no va en mayúsculas, mientras que la referencia al paquete importado, sí.  
***
Una vez que tengamos todo esto, el codigo del componente Navbar se deberia ver así:
![navbarr](/Imagenes/navbarr.png)  
Proptypes nos da un gran cúmulo de opciones que podemos usar, porque no solo podemos definir el tipo de dato que se espera recibir en una prop, sino que tmb **podriamos definir** que dicha prop es **obligatoria**, o que esperamos **recibir un array de cierto tipo de dato**, o que esa prop **puede recibir uno de varios datos posibles.**

# DefaultProps #
Las DefaultProps sirven para definir los valores por defecto que tendrá una prop en un componente. No hace falta instalar nada porque esta funcionalidad viene por defecto con cualquier componende de React.  
Para esto, dentro del mismo archivo del componente, y antes de la exportación del mismo, vamos a asignar al componente, una propiedad llamada **defaultProps**, a la cual tmb le vamos a asignar como valor un **objeto literal**.  
_Dentro de este objeto literal_, vamos a tener que hacer referencia al **nombre de la prop** y le asignamos el valor por defecto que queremos que la prop tenga, usando el paquete **prop types.**  
Por ejemplo, si tenemos el componente **saludo**, con dos props, una llamada **título** y otra **mensaje**, y queremos definir el valor por defecto para cada prop, tendriamos que hacer algo así:  
![defaultProps](/Imagenes/defaultProps.png)  
Esto lo que nos permite, es definir valores por defecto para cada propiedad que vos quieras, en el caso en que las mismas no reciban un valor al momento en que el componente es utilizado.  
>Es una manera elegante de evitar que la renderizacion de los componentes fallen por la omisión de valor para alguna de sus props.  
***
![ejer](/Imagenes/ejer.png)
![ejer1](/Imagenes/ejer1.png)
![ejer2](/Imagenes/ejer2.png)
![ejer3](/Imagenes/ejer3.png)
![ejer4](/Imagenes/ejer4.png)
![ejer5](/Imagenes/ejer5.png)  
## SLIDES ##
![slideproptype1](/Imagenes/slideproptype1.png)  
![slideproptype2](/Imagenes/slideproptype2.png)  
![slideproptype3](/Imagenes/slideproptype3.png)  
![slideproptype4](/Imagenes/slideproptype4.png)  
![slidedp1](/Imagenes/slidedp1.png)  
![slidedp2](/Imagenes/slidedp2.png)  