# Styling #
Hay **dos caminos** para introducir CSS en React.
Como bien sabemos, toda la app de React se renderiza en un archivo que se encuentra dentro de la carpeta public, llamada index.html. Es acá donde nosotros podíamos vincular nuestra hoja de estilo, siempre y cuando esta se encuentre tmb en la carpeta public. De ahí para adelante, una vez vinculada la stylesheet, todo sigue normal, como siempre.  
La única diferencia es que cuando querramos aplicar una clase dentro de un componente, deberemos usar el atributo **className** en lugar de **class**.  

React nos permite tener una hoja de estilo por componente, permitiendonos separar la presentacion visual de cada componente en distintos archivos css, con lo que ahora tendremos todo más controlado, ya que esa hoja de estilo pertenece a ese solo componente y no a toda la app.  
Cabe resaltar que esto no nos va a permitir usar los mismos nombres de clases entre componentes, porque el principio de css se siga manteniendo.
>Para que entre componentes no se pisen las reglas de estilo, tener cuidado con los nombres de las clases.
***
Para importar la hoja de estilo hacemos: 

      import './EstilosDelComponente.css'  

![styling1](/Imagenes/styling1.png)
![styling2](/Imagenes/styling2.png)
![pasoapaso](/Imagenes/pasoapaso.png)

## Otras formas de agregarr estilos ##
Existen al menos dos maneras más de agregar estilos a nuestros componentes:

- *Estilos inline*
- *styled-components*  

Veamos un poco sobre cada una de ellas.
## Estilos inline ##
De la misma manera que agregamos clases a nuestros componentes usando className, podemos agregar *estilos inline* usando el atributo *style*:
![styling3](/Imagenes/styling3.png)
En el código del ejemplo anterior, podemos notar **dos cosas**:

**Primero**, podemos ver que hay dos pares de llaves **{}** porque estamos renderizando contenido escrito en JSX. El primer par de llaves **inyecta JavaScript dentro JSX**, mientras que el par siguiente **crea un objeto literal**. Esto nos lleva a la ***segunda*** cosa interesante.

Los estilos se pasan como **objetos**, por lo que **las propiedades están separadas por comas**, pues son atributos de un objeto.

Nuestro código **ya no es CSS** sino que son **objetos Javascript**, que refieren a atributos CSS escritos de otra forma: en lugar de usar palabras separadas por guiones, como en background-color, **los escribimos usando camel case (backgroundColor).**

Al usar objetos, podemos mejorar un poco el orden de nuestro código **declarando un objeto que podemos pasar al atributo style.**
![styling4](/Imagenes/styling4.png)
Esta técnica nos permitiría **extraer todos estos objetos en un nuevo archivo**, llamémosle **styles.js**, que **podríamos importar en más de un componente** de nuestra app, favoreciendo la **reutilización del código.**
## Styled Components ##
Con **styled-components**, podemos escribir **CSS de verdad** en nuestros archivos JavaScript. Esto nos habilita a usar **todas las características de CSS** como media queries, pseudo selectores, nesting, etc.

**Styled Components** utiliza las **plantillas literales** de ES6 para estilizar componentes, eliminando el mapeado entre componentes y estilos. Con esta técnica, **cuando definimos nuestros estilos, también estamos definiendo nuestros componentes con los estilos incluidos.**

Para usar styled-components, necesitamos instalar un paquete externo a React

        npm install --save styled-components
Luego, debemos importar este paquete  

        import styled from 'styled-components';
para poder empezar a usarlo y crear nuestro primer componente:  

        const Saludo = styled.div`
        background-color: #8C8C00;
        width: 300px;
        min-height: 200px;
        `;
Veamos cómo se usa este componente.

        function SaludoApp() {
        . . .
        return (
        <Saludo>
        <h2>Hola!??</h2>
        </Saludo>
        );
        }