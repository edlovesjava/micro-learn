# Welcome to Learning Microservices

Creating an application using microservices architecture with Angular and Spring, and Docker.

## Why in the heck...

Well, I love learning stuff, and I like to learn 'out loud' so to speak, by writing tutorials or teaching others. 
This helps me to think, rememver and pause to document what I did. And others may be helped too.
I know Java with J2EE and Maven pretty well. I also Know Angular 1.5 intermedeately, and JavaScript and I are not
close friends but we are getting thee. I have generally developed monolythic architectures (but highly distributed)
on heavy weight containers, but recently have enjoyed development with the MEAN stack. Today, I believe it is 
critical for architects to understand microservices, containers (eg. docker) and cloud infrastructures and platforms.
This application will be my trail into these architectural concepts. 

# What I am doing

## Basc App - SPA / MVVM connecting to REST service

1. Start with a basic spring boot application using Gradle (yes gradle, need to learn this too!)
2. Serve static content within the spring boot starter, simple Spring MVC back end to serve static content
3. Serve the angular starter kit, remembering that it is bower / nodejs based, not gradle
4. Add node js stuff to gradle, and add automatic debendency injuection of bower to index.html links!

## Data service (Spring Data REST to Mongo DB via JPA)

5. Create a multi project gradle to serve front end, back end and additional services
6. Create a spring mvc back end, connecting on other port, allowing CORS to connect frontend (9000) to back end (8080)
7. Create a spring data REST service accessing a MongoDB server, and dockerize 
8. Run mongodb in its own container (yes, docker) and connect the service to the db resource, parameterize connect and configure

## Adding a Gateway, prep for additional services

6. Impleent [Gateway pattern](http://kubecloud.io/apigatewaypattern/) using [spring and Netflix Zuul and Spring Clud](http://kubecloud.io/apigatewaypattern/) 

