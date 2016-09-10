## Full Stack Fest 2016 - Notes

On September 8ᵗʰ and 9ᵗʰ i assisted to the **Front-end** days of the [Full Stack Fest](https://2016.fullstackfest.com/agenda/) in Barcelona (Beatifull city, i totally recommend to you) thanks to my company [BEEVA](https://www.beeva.com/en/) that allows me this to assit.  
Next i will resume to you the most important things discussed from my point of view.

**Javascript** has evolved insanely the last 5 years, the era of the [Web Apps](https://en.wikipedia.org/wiki/Web_application) is here and now the browser allows us to make Native Apps with only Javascript, HTML and CSS.
The [speakers](https://2016.fullstackfest.com/speakers/) in different ways remark that there is much more than simple web pages today, we can we built Apps in browser available for any devices out there, with **native support** for push notifictions, local storage, sync, webworkers, and why not [serverless](http://martinfowler.com/articles/serverless.html). That combined with last available JS features *thanks to Transpilers*¹, functional programming, components, etc give us incredible power to create awesome user interfaces right now.  
This technologies keep evolving and some of then even aren't supported yet by all major browsers, but things are getting better, really.

Next i will resume you some of the most important ideas and concepts talked in the fest.

#### Immutable User Interfaces by [Lee Byron](http://leebyron.com/)

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



#### Confident Frontend with Elm by [Jack Franklin](https://2016.fullstackfest.com/speakers/jack-franklin/)

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

#### The future of ES6 by [Jafar Husain](https://2016.fullstackfest.com/speakers/#jafar-husain)
This man speak fast but properly and accurated, he give an awesome talk about new JS features
> that we can and should use for the good of the Web and javascript

We should take a look and start using right now [Babel](https://babeljs.io/) it allow us to use code of the "future" not yet supported by all Browser in our Web Apps.  

Here some concepts and new features:
- Async and Await
- Async iterators
- Observer for Async iterators in browser

#### The frontend is a Full Stack by [António Nuno Monteiro](https://2016.fullstackfest.com/speakers/#antonio-nuno-monteiro)
I think we all have an idea of what this was about, the front-end is since quite a time now a Full Stack environment, we take to the **client** almost the entire logic of our Apps, there two important things that we can already work on:

- Offline WebApps
  - no need to be attached all the time to the network, we can cache, use web workers, etc
- Progressive Web Apps
  - State
  - Query for data requests  
  - Data binding comes to observing
  - Virtual DOM for speed
  - HTTP 2

#### See the data flowing through your app by André Staltz
André mades [cycle.js](http://cycle.js.org/) in its free time, is a framework that allows us to see the behavior of our Apps in an more convenient way, we don't want to see all the details chrome debug like, we want the important things only to get a big picture.

#### Others ideas
There was a lot of more interesting ideas like [use service workers to comunicate different Tabs](https://2016.fullstackfest.com/speakers/andrew-dunkman/), [CSS 4 Grid](https://2016.fullstackfest.com/speakers/jen-kramer/) (for designers), PouchDB, WebRTC and of course [WebAssembly](https://2016.fullstackfest.com/speakers/bensmith/) a shorcut to the Javascript compiler, yes, future looks promising.

Hope you can dig in on the topics you liked most, i
leave you with this question that came out in some talks:

> Do you think Safari is the new IE ?

Answer me on twitter [@juliomatcom](https://twitter.com/juliomatcom)

¹ Yes you will keep using [Babel](https://babeljs.io/) if you want to try and use lastests features
