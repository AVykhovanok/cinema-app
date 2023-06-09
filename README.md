# CINEMA<br>


## About a project
Cinema service is a basic web application for online booking of cinema tickets. 
It represents the work of a cinema service and providing the possibility of user 
registration and authentication, as well as all CRUD operations with order, 
shopping cart, movie, movie session and cinema hall.The web application consists 
of backend part, it implemented using n-tiered architecture in accordance with 
SOLID and REST principles.
***

## Features
Registration:<br>
```
POST: /register
```

All roles:<br>
```
GET:/cinema-halls - watch all cinema-halls
```
```
GET:/movie-sessions/available - watch all available movie sessions
```
```
GET:/movie-sessions / {id} - watch a certain movie session
```
```
GET:/logout - log out
```

Administration:<br>
```
POST:/cinema-halls - add a new cinema-halls
```
```
POST:/movies - add a new movie
```
```
POST:/movie-sessions - add a movie session
```
```
PUT:/movie-sessions/{id} - update information about a movie session
```
```
DELETE:/movie-sessions/{id}  - delete movie session
```
```
GET:/users/by-email - get a user by mail
```

User:<br>
```
GET:/orders - get your orders
```
```
GET:/shopping-carts/by-user - get your shopping cart
```
```
POST:/orders/complete - complete the order
```
```
PUT: /shopping-carts/movie-sessions - add movie ticket to cart
```

***
## Model structure
![Schema](Hibernate_Cinema_Uml.png)
***


## Technologies

* Java - 17
* Hibernate - 5.6.14.Final
* Spring - 5.6.10
* MySQL -  8.0.33
* Apache Tomcat - 9.0.74
***

## Setup.

__Steps__
* Clone this repo
* Create schema in your "MySQL Workbench"
* Add your personal info to db.properties to connect to your database.
* Add Tomcat 9.0.50 configuration.
