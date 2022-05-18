## REACT ##
Es una biblioteca para Javascript pensada para crear proyectos del lado del frontend. Su implementación permite que la carga de la app sea más rápida, optimizada y performante.  
Para lograrlo **React** usa **componentes**, que son bloques de código REUTILIZABLES que creamos una sola vez y luego los usamos cuando y donde sea necesario.  
***
>React vio la luz en marzo del 2013 de la mano de Jordan Walke, Ingeniero de Software en Facebook. Su primera implementación fue en el timeline de Facebpk, ya que en su momento buscaban una manera óptima y rápida de cargar los contenidos en su red social._
***
La libreria trabaja con un concepto llamado __virtual DOM__. Este se basa en una idea bastante sencilla e ingeniosa. Sencillamente consta en tomar una copia exacta del DOM real _(interfaz de objetos que interpreta nuestro HTML, sirve para acceder a nuestros elementos y poder manipularlos)_ y comparar las mismas contantemente. Y justo cuando sucede un cambio, es decir, cuando cambia el estado de la app, dicha copia será actualizada.  
Es aquí el momento de __comparar__ el virtual DOM con el DOM real. Cuando React sabe perfectamente qué partes de la página debe actualizar, se ahorra la necesidad de actualizar la vista completa.  
Es algo muy potente que hace de manera automática y que aumenta fuertemente el rendimiento de los componentes y de toda nuestra app en el frontend.  
Este proceso de _comparar_ las dos versiones del DOM se llama __DIFFING__ y el proceso de _actualización_ recibe el nombre de __RECONCILIATION__.  
De esta maneta labura React. Si bien no es obligacion usarlo, es altamente _recomendable_ para optimizar todas nuestras vistas del lado del front.