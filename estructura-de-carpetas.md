## Estructura de carpetas ##
Comencemos a desarmar parte por parte todos los elementos que componen un proyecto en React en términos de carpetas y archivos relevantes. Así se debería ver el directorio de nuestro proyecto una vez ejecutados los comandos **npx create-react-app “mi-proyecto”**, luego **cd “mi-proyecto”**, y por último **npm start**.  

![Carpetas](/Imagenes/carpetas.png)  

![Node_modules](/Imagenes/node.png)

![Public](/Imagenes/public.png)

![Src](/Imagenes/src.png)

![Package.json](/Imagenes/package.png)
***
## ¿Cómo convive la estructura MVC con React? ##
Todo muy lindo con React, pero ¿cómo encaja dentro del esquema MVC?

React viene a ser la V dentro de este patrón de diseño, es decir, todo lo que hagamos con React está pensado para ser las vistas de nuestra aplicación.

Hasta ahora, todo lo habíamos construido directamente dentro de Express y desde allí respondíamos a las peticiones hechas por el cliente con las vistas, pero antes de que la vista viajara al navegador necesitábamos dejar todo listo (datos, variables y demás).

Ahora, con la potencia que nos dan las APIs, vamos a poder construir todo el front-end con React y consumir los datos del back-end a través de peticiones asincrónicas. De esa manera podremos separar radicalmente la lógica del back-end de la lógica del front-end.