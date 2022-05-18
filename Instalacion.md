# Instalación y puesta en marcha #
>"Al ser una librería de JavaScript, React pertenece al conjunto de paquetes que gestiona __npm i__ para instalar el ambiente de desarrollo."  

Existen muchas formas para inicializar una app React. Nosotros usaremos la herramienta __Create React App (CRA)__, un ambiente cómodo para aprender React que, además, es la mejor manera de comenzar a construir una nueva SPA usando React.

__CRA__ configura nuestro ambiente dde desarrollo habilitando las últimas características de JS, brindando una buena experiencia de desarrollo y, optimizando nuestra app para producción.

>***Para usar CRA, necesitamos tener Node 14.0.0 y npm 5.6 instalados en nuestra compu.***  
***

## Vamos a crear nuestra primera app React. ##
1. Lo primero que necesitamos hacer es ubicarnos en la carpeta en donde queremos que se guarde el proyecto.
2. Luego, desde la terminal ejecutamos el comando __npx create-react-app my-app__ reemplazando __my-app__ por el nombre de nuestra app ___(no puede contener espacios y se recomienda escribir todo en minúsculas, separando las palabras por guiones)___  
  
  Una vez hecho esto, React tomará unos minutos para descargar los paquetes y dependencias necesarios para iniciar nuestra app.  
    
Finalizado este proceso, estaremos en condiciones de __probar nuestra nueva app.__  
  
Usando el comando cd my-app (recuerda cambiar my-app por el nombre de tu app) nos moveremos al directorio generado por React con la estructura de archivos de nuestra app.   
![Ract](ReactComandos.png)
***

## ¿Cómo evitamos que se cree una nueva carpeta? ##
  A veces, queremos que nuestra aplicación React se cree directamente en el directorio en el que estamos trabajando y no dentro de una nueva carpeta. Podemos lograr este comportamiento usando el comando de la siguiente forma:  
  
    npx create/react/app .  
    
Si observamos detenidamente, podemos ver que cambiamos el nombre del nuevo directorio por un punto (.). Esto funcionará correctamente siempre que el nombre de la carpeta en donde ejecutemos el comando cumpla con las siguientes reglas:
- Contiene sólo caracteres compatibles con una URL.
- No tiene letras mayúsculas.  

Por ej, no podemos nombrarla con "React App", lo correcto es "react-app".
***

## ¿Por qué usamos Create React App con npx?
Dado que ***create-react-app*** es un paquete de Node.js que deseamos ejecutar sólo una vez por cada proyecto no buscamos instalarlo permanentemente, sino que tiene sentido descargarlo y ejecutarlo al vuelo para luego continuar con lo que nos interesa. Además de esta forma, nos aseguramos de utilizar la última versión disponible. ¡Sencillo, ágil y al día!
***
## Estructura de carpetas ##
Comencemos a desarmar parte por parte todos los elementos que componen un proyecto en React en términos de carpetas y archivos relevantes. Así se debería ver el directorio de nuestro proyecto una vez ejecutados los comandos **npx create-react-app “mi-proyecto”**, luego **cd “mi-proyecto”**, y por último **npm start**.  

![carpteas](/imagenes/carpetas.png)  

![node_modues](/imagenes/node.png)

![public](/imagenes/public.png)

![src](/imagenes/src.png)

![package.json](/imagenes/package.png)  
***
## ¿Cómo convive la estructura MVC con React? ##
Todo muy lindo con React, pero ¿cómo encaja dentro del esquema MVC?

React viene a ser la V dentro de este patrón de diseño, es decir, todo lo que hagamos con React está pensado para ser las vistas de nuestra aplicación.

Hasta ahora, todo lo habíamos construido directamente dentro de Express y desde allí respondíamos a las peticiones hechas por el cliente con las vistas, pero antes de que la vista viajara al navegador necesitábamos dejar todo listo (datos, variables y demás).

Ahora, con la potencia que nos dan las APIs, vamos a poder construir todo el front-end con React y consumir los datos del back-end a través de peticiones asincrónicas. De esa manera podremos separar radicalmente la lógica del back-end de la lógica del front-end.