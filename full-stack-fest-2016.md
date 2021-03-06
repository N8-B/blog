## [Full Stack Fest 2016](https://youtu.be/vxMASndC3k4?list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - Notes

On September 8ᵗʰ and 9ᵗʰ I assisted to the **Front-end** days of the [Full Stack Fest](https://2016.fullstackfest.com/agenda/) in Barcelona (Beatifull city, I totally recommend to you) thanks to my company [BEEVA](https://www.beeva.com/en/) that allows me this to assit.  

**Javascript** has evolved insanely the last 5 years, the era of the [Web Apps](https://en.wikipedia.org/wiki/Web_application) is here and now the browser allows us to make Native Apps with only Javascript, HTML and CSS.
The [speakers](https://2016.fullstackfest.com/speakers/) in different ways remark that there is much more than simple web pages today, we can we built Apps in browser available for any devices out there, with **native support** for push notifictions, local storage, sync, webworkers, and why not [serverless](http://martinfowler.com/articles/serverless.html). That combined with last available JS features *thanks to Transpilers*¹, functional programming, components, etc give us incredible power to create awesome UIs right now.  
This technologies keep evolving and some of then even aren't supported yet by all major browsers, but things are getting better, really.

Next I will resume you some of the most important ideas and concepts talked in the fest.

#### [Immutable User Interfaces](https://www.youtube.com/watch?v=pLvrZPSzHxo&index=18&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Lee Byron](http://leebyron.com/)

##### Architectures
 **MVC** don't resolves our problems today because of the cost of made a whole controller be aware of the changes of the View, instead he propose the adoption of the **Inmutable App Architecture** with implies:
  - Tiny changes
  - Component oriented.
  - Functional Programming
  - Virtual Dom
  - (state) => View

*Slide pictures comming soon*

#####  Network
In the side of the **requests** to the server we see the decline of the Rest APIs for new ideas

**Rest**:   
Makes very difficult gets the resources we need in less Requests and the consequences it brings like, more requests to the server, more time waiting, worst and slower user interfaces.

**GraphQL and query in Frontend**:  
Grab more data in every request,  cache it, works with offline experience.

With this factor we can simplify Web Apps challenges and leverage principles of inmutability. Is important to use [InmutableJS](https://github.com/facebook/immutable-js) for speed and meomization

<a href="http://www.youtube.com/watch?feature=player_embedded&v=pLvrZPSzHxo" target="_blank"><img src="http://img.youtube.com/vi/pLvrZPSzHxo/0.jpg" 
alt="Immutable User Interfaces (Lee Byron) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>


#### [Confident Frontend with Elm](https://www.youtube.com/watch?v=rDQ22Yg3Fms&index=19&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Jack Franklin](https://2016.fullstackfest.com/speakers/jack-franklin/)

[Elm](http://elm-lang.org/) is a functional language that compiles to JavaScript. It competes with projects like React as a tool for creating websites and web apps.  

Some of the goods of this languajes remarked by Jack are:
- Components over ~~controllers~~
- Data flow in **one** direction
- A view represent a **state**

Plus the native advantages of be functional, typed and compiled allow us to a avoid lot of **bad things** like:
- Impure functions
- Errors during ejecution   
  like the classic *Something is Undefined* in js
- Mutability

It was a nice talk about how Elm can change the way we build Web Apps in the future, but for now not even Jack recommend to use Elm in production.

<a href="http://www.youtube.com/watch?feature=player_embedded&v=rDQ22Yg3Fms
" target="_blank"><img src="http://img.youtube.com/vi/rDQ22Yg3Fms/0.jpg" 
alt="Confident Frontend with Elm (Jack Franklin) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>

#### [The future of ES6](https://www.youtube.com/watch?v=3pKNRgResq0&index=20&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Jafar Husain](https://2016.fullstackfest.com/speakers/#jafar-husain)
This man speak fast but properly and accurated, he give an awesome talk about new JS features
> that we can and should use for the good of the Web and javascript

We should take a look and start using right now [Babel](https://babeljs.io/) it allow us to use code of the "future" not yet supported by all Browser in our Web Apps.  

Here some concepts and new features:
- Async and Await
- Async iterators
- Observer for Async iterators in browser 

<a href="http://www.youtube.com/watch?feature=player_embedded&v=3pKNRgResq0
" target="_blank"><img src="http://img.youtube.com/vi/3pKNRgResq0/0.jpg" 
alt="The future of ES6 (Jafar Husain) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>

#### [The frontend is a Full Stack](https://www.youtube.com/watch?v=wtURpqTgtUs&index=23&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [Luca Marchesini](https://2016.fullstackfest.com/speakers/luca-marchesini/)
I think we all have an idea of what this was about, the front-end is since quite a time now a Full Stack environment, we take to the **client** almost the entire logic of our Apps, there two important things that we can already work on:

- Offline WebApps
  - no need to be attached all the time to the network, we can cache, use web workers, etc
- Progressive Web Apps
  - State
  - Query for data requests  
  - Data binding comes to observing
  - Virtual DOM for speed
  - HTTP 2  

<a href="http://www.youtube.com/watch?feature=player_embedded&v=wtURpqTgtUs
 " target="_blank"><img src="http://img.youtube.com/vi/wtURpqTgtUs/0.jpg" 
 alt="The Frontend Is a Full Stack (Luca Marchesini) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>
 
#### [See the data flowing through your app](https://www.youtube.com/watch?v=R-GzJgEccEQ&index=27&list=PLe9psSNJBf76DOOKMkDpyo_A5PfZk7JWc) - [André Staltz](https://2016.fullstackfest.com/speakers/andre-staltz/)
André mades [cycle.js](http://cycle.js.org/) in its free time, is a framework that allows us to see the behavior of our Apps in an more convenient way, we don't want to see all the details chrome debug like, we want the important things only to get a big picture. 

<a href="http://www.youtube.com/watch?feature=player_embedded&v=R-GzJgEccEQ
" target="_blank"><img src="http://img.youtube.com/vi/R-GzJgEccEQ/0.jpg" 
alt="See the data flowing through your app (André Staltz) - Full Stack Fest 2016" width="240" height="180" border="10" /></a>	

#### Others ideas
There was a lot of more interesting ideas like [use service workers to comunicate different Tabs](https://2016.fullstackfest.com/speakers/andrew-dunkman/), [CSS 4 Grid](https://2016.fullstackfest.com/speakers/jen-kramer/) (for designers), PouchDB, WebRTC and of course [WebAssembly](https://2016.fullstackfest.com/speakers/bensmith/) a shorcut to the Javascript compiler, yes, future looks promising.

Hope you can dig in on the topics you liked most, i
leave you with this question that came out in some talks:

> Do you think Safari is the new IE ?

Answer me on twitter [@juliomatcom](https://twitter.com/juliomatcom)

¹ Yes you will keep using [Babel](https://babeljs.io/) if you want to try and use lastests features
