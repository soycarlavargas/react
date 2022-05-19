# Props #
>Las **props** son entradas de un componente de React. Representan info que es pasada desde un **componente padre** a un **componente hijo**. Pueden recibir *propiedades* como parámetros para poder insertar valores y eventos en HTML.
***  
Las **props** son tmb conocidas como ***propiedades de un componente***. Una **propiedad** es un valor que se envia al componente al momento en que este mismo se llama o implementa. Todo componente tiene la posibilidad de recibir sus props por parametro al momento en que se está creando el mismo. Este parámetro será un objeto literal que contiene a todas las propiedades que sean pasadas al componente al momento de su uso. Es por eso que al momento de crear el componente, lo primero que hay que hacer es pasar un parametro llamado PROPS.  
Luego, lo que hay que hacer dentro del componente es imprimir la propiedad deseada en el lugar indicado.  
![props](/Imagenes/props1.png)  
Lo que hay que hacer dentro del componente, es imrpimir la prop deseada en el lugar indicado. A través de las llaves indicamos en qué lugares queremos poner el valor de las propiedades cuando las mismas se envían.  
![props2](/Imagenes/props2.png) 
Ahora el componente saludo es una pieza de codigo 100% reutilizable. Su contenido ahora va a cambiar segun el valor de sus propiedades.  

## Implementación ##
Las propiedades de un componente, reciben sus respectivos valores cuando el componente es INVOCADO por la app. Pensa que este componente saludo es importado dentro del componente principal App. Es aqui, en este momento cuando decidis usar el componente, donde le daras valor a las propiedades.  
Al componente le tenes que config en forma de atributo HTML el nombre de la prop y el valor que le querés dar.  
![props3](/Imagenes/props3.png)  
De esta manera, ya podes hacer que un componente al momento de ser utilizado, reciba por parámetro distintos valores.  
![props4](/Imagenes/props4.png)
![props5](/Imagenes/props5.png)
![props6](/Imagenes/props6.png)   
![props7](/Imagenes/props7.png)  
  
  ## Slides de props ##
![props8](/Imagenes/props8.png) 
![props9](/Imagenes/props9.png) 
![props10](/Imagenes/props10.png) 



