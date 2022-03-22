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
java -jar target/notes-app-rest-api-1.0.0.jar
```

Alternatively, you can run the app without packaging it using:
```mvn spring-boot:run```

The app will start running at http://localhost:8080.

# Exploring the REST API
The following explores the CRUD (Create, Remove, Update AND Delete) operations this application supports. In the screenshots below, I am using Postman to perform the API calls.

1. Get all notes using GET method:
```
GET localhost:8080/api/v1/notes
```
![Screen Shot 2022-03-22 at 7 16 21 pm](https://user-images.githubusercontent.com/79638487/159440138-4ee68467-c890-440d-a474-b510c8ab6601.png)

2. Get note with a specific ID using GET method:
```
GET localhost:8080/api/v1/notes/{noteId}
```
In the screenshot below, we are returning the note with the ID of ```1```
![Screen Shot 2022-03-22 at 7 16 55 pm](https://user-images.githubusercontent.com/79638487/159440535-b0ebe6d6-e0be-4e1c-8703-4ed629e98e3f.png)

3. Add a note using POST method:
```
POST localhost:8080/api/v1/notes
```
In the screenshot below, we are adding a new note
![Screen Shot 2022-03-22 at 7 14 17 pm](https://user-images.githubusercontent.com/79638487/159441624-bbec2ff6-8568-433f-9fb8-ef2fc87335d2.png)

4. Update an existing note using PUT method:
```
PUT localhost:8080/api/v1/notes/{noteId}
```
In the screenshot below, we are updating the note with the ID of ```2```
![Screen Shot 2022-03-22 at 7 18 11 pm](https://user-images.githubusercontent.com/79638487/159441811-03a2342d-f023-437a-80ea-e8b308a80f76.png)

5. Delete a note using DELETE method:
```
DELETE localhost:8080/api/v1/notes/{noteId}
```
In the screenshot below, we are deleting the note with the ID of ```2```
![Screen Shot 2022-03-22 at 7 18 38 pm](https://user-images.githubusercontent.com/79638487/159442004-58243fa3-08c7-4b5b-8e0c-207830daa761.png)
