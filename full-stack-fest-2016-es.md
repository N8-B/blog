### [Full Stack Fest 2016](https://youtu.be/vxMASndC3k4?list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc)
Los ponentes remarcaron de diferentes maneras que hay mucho más que simple páginas web hoy, ahora podemos desarrollar Apps en el navegador disponibles para todos los dispositivos, con **soporte nativo** para notificaciones Push, local storage, sync, web workers y porque no serverless. Esto combinado con las últimas features de Javascript (Gracias a los transpiladores), programación funcional, componentes, etc nos dan la posibilidad de crear interfaces de usuarios increibles.

#### [Immutable User Interfaces](https://www.youtube.com/watch?v=pLvrZPSzHxo&index=18&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Lee Byron](http://leebyron.com/)

##### Arquitecturas
**MVC** no resuelve nuestros problemas de hoy, debido al costo de hacer que todo un **controlador** este al tanto de todos los cambios en la **Vista**, Lee propone la adopcón de la **Immutable App Architecture** que implica:	

 - Pequeños cambios
 - Orientado a componentes
 - Programación funcional
 - Virtual DOM
 - (estado) => Vista

##### Red
En el lado de las peticiones al servidor vemos un declive hacia las Apis Rest

- **Rest**	
	Hace difícil obtener los recursos en menos peticiones trayendo consigo consecuencias como, más peticiones al servidor, más tiempo de espera, una peor experiencia de usuario.
- **GraphQL**	
	Obtienes mas datos en cada petición al servidor, se pueda cachear, permite una experiencia offline	
	
Con estos factores podemos simplificar los retos de desarrollar WebApps e incrementar los principios de inmutabilidad. Es importante usar [ImmutableJS](https://github.com/facebook/immutable-js) para una mayor eficiencia, al igual que meomization.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=pLvrZPSzHxo" target="_blank"><img src="http://img.youtube.com/vi/pLvrZPSzHxo/0.jpg" 
alt="Immutable User Interfaces (Lee Byron) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>

#### [Confident Frontend with Elm](https://www.youtube.com/watch?v=rDQ22Yg3Fms&index=19&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Jack Franklin](https://2016.fullstackfest.com/speakers/jack-franklin/)

[Elm](http://elm-lang.org/) es un lenguaje funcional que compila a Javascript. Compite con proyectos como React en el desarrollo de Web Apps.

Algunas bondades del lenguaje destacadas por Jack son:

 - Componentes y no ~~controladores~~
 - Los datos fluyen en **una** dirección
 - Una vista representa un **estado** 

Sumado a la ventaja nativa de ser funcional, tipado y compilado nos permite evitar muchos problemas como:

 - Funciones impuras
 - Errores en ejecución	
 	 ej: El clásico *algo es undefined en JS*
 - Mutabilidad

Fue una buena charla de como Elm puede cambiar la manera en que desarollamos aplicaciones Web en el futuro, pero por ahora ni siquiera Jack recomienda usar Elm para producción.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=rDQ22Yg3Fms
" target="_blank"><img src="http://img.youtube.com/vi/rDQ22Yg3Fms/0.jpg" 
alt="Confident Frontend with Elm (Jack Franklin) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>
 

#### [The future of ES6](https://www.youtube.com/watch?v=3pKNRgResq0&index=20&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Jafar Husain](https://2016.fullstackfest.com/speakers/#jafar-husain)

Este hombre habla rápido, pero claro y conciso, ha dado una increible charla de las nueva "features" de JS

> ...que podemos y deberíamos usar por el futuro de Javascript y la Web

Nos comenta que debemos usar [Babel](https://babeljs.io/) el cual nos permite usar código del "futuro" que aún no está soportado en todos los navegadores.	

Estos son algunos conceptos que recomienda mirar:
 - Async y Await
 - Async iterators
 - Observers para Async iterators en el navegador
 
 <a href="http://www.youtube.com/watch?feature=player_embedded&v=3pKNRgResq0
" target="_blank"><img src="http://img.youtube.com/vi/3pKNRgResq0/0.jpg" 
alt="The future of ES6 (Jafar Husain) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>

#### [The frontend is a Full Stack](https://www.youtube.com/watch?v=wtURpqTgtUs&index=23&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Luca Marchesini](https://2016.fullstackfest.com/speakers/luca-marchesini/)
Creo que todos tenemos una idea de que se habló en esta charla, el Front-end es desde hace un tiempo un entorno Full Stack, hemos llevado al Cliente casi toda la lógica de nuestras Aplicaciones, existen 2 cosas importantes que ya podemos comenzar a utilizar:	
 - Web Apps offlines
	 - No necesitamos estar todo el tiempo conectados para que nuestra aplicacion responda correctamente
 - Aplicaciones progresivas
 	 - Estado
	 - Peticiones con queries 
	 - Data binding con observers
	 - Virtual Dom para mayor eficiencia
	 - HTTP 2	


 <a href="http://www.youtube.com/watch?feature=player_embedded&v=wtURpqTgtUs
 " target="_blank"><img src="http://img.youtube.com/vi/wtURpqTgtUs/0.jpg" 
 alt="The Frontend Is a Full Stack (Luca Marchesini) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>
	



#### [See the data flowing through your app](https://www.youtube.com/watch?v=R-GzJgEccEQ&index=27&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [André Staltz](https://2016.fullstackfest.com/speakers/andre-staltz/)

André creó [cycle.js](http://cycle.js.org/) en su tiempo libre, es un framework que nos permite ver el comportamiento de nuestra App de una manera más conveniente, no necesitamos ver todos esos detalles al estilo Debug en Chrome, queremos ver lo que nos importa para obtener un mejor *big picture*	

<a href="http://www.youtube.com/watch?feature=player_embedded&v=R-GzJgEccEQ
" target="_blank"><img src="http://img.youtube.com/vi/R-GzJgEccEQ/0.jpg" 
alt="See the data flowing through your app (André Staltz) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>	

#### Otras ideas
Hubieron muchas ideas interesantes como, [usar web workers para comunicar diferentes pestañas del navegador](https://2016.fullstackfest.com/speakers/andrew-dunkman/), [CSS 4 Grid](https://2016.fullstackfest.com/speakers/jen-kramer/) (para diseñadores), PouchDB, WebRTC, y por supuesto [WebAssembly](https://2016.fullstackfest.com/speakers/bensmith/), un acceso directo al compilador de Javascript.. 
Sin dudas el futuro en Front-end sigue prometiendo mucho.
