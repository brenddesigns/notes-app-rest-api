# Notes App REST API
Restful CRUD API for a simple note taking application using Spring Boot, Mysql, JPA and Hibernate.

# Setup 
1. Clone the application:
```
git clone https://github.com/brenddesigns/notes-app-rest-api.git
```

2. Create MySQL database:
```
CREATE DATABASE notes_app;
```

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

# Exploring the REST API

1. Get All Notes:
```
GET /api/notes
```
![Screen Shot 2022-03-22 at 7 16 21 pm](https://user-images.githubusercontent.com/79638487/159440138-4ee68467-c890-440d-a474-b510c8ab6601.png)
