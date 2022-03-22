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

1. Get all notes from MySQL database:
```
GET localhost:8080/api/v1/notes
```
![Screen Shot 2022-03-22 at 7 16 21 pm](https://user-images.githubusercontent.com/79638487/159440138-4ee68467-c890-440d-a474-b510c8ab6601.png)

2. Get specific note with a specific ID:
```
GET localhost:8080/api/v1/notes/{noteId}
```
In the screenshot below, we are returning the note with the id of ```1```
![Screen Shot 2022-03-22 at 7 16 55 pm](https://user-images.githubusercontent.com/79638487/159440535-b0ebe6d6-e0be-4e1c-8703-4ed629e98e3f.png)

3. Add a note using PUT method:
```
PUT localhost:8080/api/v1/notes/{noteId}
```
In the screenshot below, we are adding note with id of ```2```
![Screen Shot 2022-03-22 at 7 18 11 pm](https://user-images.githubusercontent.com/79638487/159441270-ce785304-3c86-4aeb-b986-e7dd91c9c6b1.png)
