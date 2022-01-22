# Cinema App
This is a web application that show a simulation of a cinema user service, authenticated user 
can have two roles USER or ADMIN.
## Implementation details in project:
* 3 layer architecture
    - Controllers
    - Services
    - DAO
* Dependency injection and Inversion of control
* RESTfull application
## Technologies used in project:
* Apache Tomcat (v9.0.55)
* Hibernate
* Spring (Web, REST, Security)
* MySQL
* JPQL
* Maven
## Available functions:
###Depends on role you can do below-mentioned functions
####ADMIN Opportunities:
* POST: /cinema-halls
* POST: /movies
* POST: /movie-sessions
* PUT: /movie-sessions/{id}
* DELETE: /movie-sessions/{id}
* GET: /users/by-email

####USER Opportunities: 
* POST: /orders/complete
PUT: /shopping-carts/movie-sessions
* GET: /orders
* GET: /shopping-carts/by-user

####Both USER / ADMIN Opportunities
* GET: /cinema-halls
* GET: /movies
* GET: /movie-sessions/available
## Recommendations to run project:
1. Intellij IDEA Ultimate Edition
2. Apache Tomcat version 9.0.55
3. MySQL and MySQL Workbench
4. In db.properties fill database fields
5. Edit your Tomcat configuration

After running tomcat in your browser opened authenticated table
feel free to use one of already created in DataInitializer 
and use Postman for noGet operations:
* for USER username = userUser@gmail.com password 123123 
* for ADMIN username = userAdmin@gmail.com password 123123 
