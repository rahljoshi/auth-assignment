# auth-assignment

This repository contains the authentication assignment.

### About Project
* I created a Spring Boot project using JWT Tokens for authentication and authorization.    
* I have used IntelliJ as my IDE for this assignment.
* I have used Spring Boot and H2 as database alongside JWT.

### How to run the project
Clone this repository can then you can open this project in any ide like IntelliJ/Eclipse and once you open it, IDE will automatically download all the required
dependencies, and after it you can run the main file **_AuthenticationApplication_** 

### Flow of the project
* After starting the project you have first to register the user. 
  * URL: http://localhost:8090/add and Request body will be in JSON format and it will have two fields username and password.
* After registering the user you have to log in and once you log in you will receive the JWT Token as a response.
  * URL: http://localhost:8090/login and request body will be in JSON format and it will have two fields username and password.
* Once you have the token then you add the token to your request and send the request, once you send the request you will receive a string as a response.
  * URL: http://localhost:8090/home


## Screenshots
