# notes-app-rest-api
Restful CRUD API for a simple note taking application using Spring Boot, Mysql, JPA and Hibernate.

# Setup 
1. Clone the application:
```git clone https://github.com/brenddesigns/notes-app-rest-api.git```

2. Create MySQL database:
```CREATE DATABASE notes_app;```

3. Change MySQL username and password inside application.properties file:
* Open ```src/main/resources/application.properties```
* Change ```spring.datasource.username``` and ```spring.datasource.password``` as per your installation.

4. Build and Run the application using Maven:
```
mvn package
java -jar target/easy-notes-1.0.0.jar
```

Alternatively, you can run the app without packaging it using:
```mvn spring-boot:run```

The app will start running at http://localhost:8080.
