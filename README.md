# Cinema App
This is a web application that show a simulation of a cinema service, authenticated user 
can have two roles USER or ADMIN.
## Implementation details of project:
* 3 layer architecture
    - Controllers
    - Services
    - DAO
* Dependency injection and Inversion of control
* RESTfull application
## Technologies used in project:
* Apache Tomcat (v9.0.55)
* Hibernate
* Spring (Core, Web, Security)
* MySQL
* Maven
## Available functions:
### Depending on the role you can use different endpoints:
#### ADMIN:
* POST: /cinema-halls
* POST: /movies
* POST: /movie-sessions
* PUT: /movie-sessions/{id}
* DELETE: /movie-sessions/{id}
* GET: /users/by-email
#### USER: 
* POST: /orders/complete
* PUT: /shopping-carts/movie-sessions
* GET: /orders
* GET: /shopping-carts/by-user
#### USER/ADMIN:
* GET: /cinema-halls
* GET: /movies
* GET: /movie-sessions/available
## Recommendations to run project:
1. Install MySQL and Apache Tomcat
2. Create an empty DB called "cinema-app"
3. Clone this project to your IDE
4. Configure src/main/resources/db.properties file for it to fit your DB
5. Add Tomcat to your project's run/debug
6. Run the project

After running tomcat in your browser opened authenticated table
feel free to use one of already created in DataInitializer 
and use Postman for noGet operations:
* for USER username = userUser@gmail.com password 123123 
* for ADMIN username = userAdmin@gmail.com password 123123 
