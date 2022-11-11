# PolyLink

## 💡 Main topic

This organization was created to do a school Project in the last of a 5-years studying computer science engineering (Polytech Montpellier, France).

The goal of this project is to create a Linkedin-like application using a microservices architecture. 

## ❔ Requirements

Here is what we were asking for :
- Jobseeker can authenticate, update his profile (adding CV), check and find offers helped by a recommendation system and apply for an offer
- Employer can manage offers and associate a jobseeker to one of its (jobseeker become an employee)
- Employee can rate the employer and vice-versa

## 🌞 Technologies and technical constraints

In order to do this, we will use :
- Spring Boot to implement the microservices logic (backend)
- ReactJS to implement the frontend
- Gradle to handle the dependencies and the build system
- Spring Mock MVC to implement the tests
- Keycloak to handle the authentication (O'Auth2 protocol)
- PostgreSQL to store our data
- Kafka to use pipeline and handle the recommendation system storage
- Docker to handle the containers of the microservices, database and modules

## 👨‍💻 Development management

Each git repository will have 3 main branches :
 - dev : used for the development
 - staging : used to test the last version of the application
 - prod : used for the deployment of the application (released version)

## 🚥 Deployment management

To deploy our application, we will use a private cluster from a server of our school (using Dokku).
Each microservice and each module will be build and run in a single container. 
Only the frontend and the gateway microservice containers will be exposed to external requests (internet).
The containers will communicate together using an internal network.

## 👊 Your turn !

Now, we let you check on your side our different repositories, have fun !!!

###### created by Alexandre FERNIQUE & Quentin DESBROUSSES in 2022