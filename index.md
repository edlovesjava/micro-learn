# Welcome to Learning Microservices

Creating an application using microservices architecture with Angular and Spring, and Docker.

## Why in the heck...

Well, I love learning stuff, and I like to learn 'out loud' so to speak, by writing tutorials or teaching others. 
This helps me to think, rememver and pause to document what I did. And others may be helped too.
I know Java with J2EE and Maven pretty well. I also Know [Angular 1.5](https://angularjs.org/) intermediately, and [JavaScript](https://en.wikipedia.org/wiki/ECMAScript) and I are not
close friends but we are getting there. I have generally developed [monolithic architectures](http://microservices.io/patterns/monolithic.html) (but highly distributed)
on heavy weight [J2EE containers](http://docs.oracle.com/cd/E17904_01/web.1111/e13706/overview.htm#WLPRG107), but recently have enjoyed development with the [MEAN stack](https://meanjs.org/) ([MongoDB](https://www.mongodb.com/), [Express](http://expressjs.com/), [Angular](https://angularjs.org/) and [Node](https://nodejs.org/en/)). Today, I believe it is 
critical for architects to understand[ microservices architecture](http://microservices.io/patterns/microservices.html), containers (eg. docker) and cloud infrastructures and platforms.
This application will be my trail into these architectural concepts. 

# What I am doing?

## Phase 1 - Basic Pattern

![MS Phase 1](Microservice example p1.png)

### Basc App - SPA / MVVM connecting to REST service

1. Start with a basic spring boot application using Gradle (yes gradle, need to learn this too!)
2. Serve static content within the spring boot starter, simple Spring MVC back end to serve static content
3. Serve the angular starter kit, remembering that it is bower / nodejs based, not gradle
4. Add node js stuff to gradle, and add automatic debendency injuection of bower to index.html links!

### Data service (Spring Data REST to Mongo DB via JPA)

5. Create a multi project gradle to serve front end, back end and additional services
6. Create a spring mvc back end, connecting on other port, allowing CORS to connect frontend (9000) to back end (8080)
7. Create a spring data REST service accessing a MongoDB server, and dockerize 
8. Run mongodb in its own container (yes, docker) and connect the service to the db resource, parameterize connect and configure

### Adding a Gateway, prep for additional services

9. Impleent [Gateway pattern](http://kubecloud.io/apigatewaypattern/) using [spring and Netflix Zuul and Spring Clud](http://kubecloud.io/apigatewaypattern/) 

