# auth-assignment

This repository contains the authentication assignment.

### About Project
* I created a Spring Boot project using JWT Tokens for authentication and authorization.    
* I have used IntelliJ as my IDE for this assignment.
* I have used Spring Boot and H2 as database alongside JWT.

### How to run the project
Clone this repository can then you can open this project in any ide like IntelliJ/Eclipse and once you open it, IDE will automatically download all the required
dependencies, and after it you can run the main file **_AuthenticationApplication_** 

## Project Structure
* _config_ package contains security-related configurations, like Authentication Manager, configuring endpoints that should be authorized and which should not.
* _controller_ package contains two controllers home controller and the user controller.
* _filter_ package contains JwtFilter class which is used to filter the token from the incoming request and then send it ahead for validating it.
* _model_ package contains models which are required for the project which are User and JWTResponse classes.
* _repository_ package contains repository classes for the models.
* _service_ package contains the User service class which is the service layer that performs actions on the User model.
* _utility_ package contains JWTUtility class which basically helps to generate tokens, validate them, expire the token, etc.

### Flow of the project
* After starting the project you have first to register the user. 
  * URL: http://localhost:8090/add and Request body will be in JSON format and it will have two fields username and password.
* After registering the user you have to log in and once you log in you will receive the JWT Token as a response.
  * URL: http://localhost:8090/login and request body will be in JSON format and it will have two fields username and password.
* Once you have the token then you add the token to your request and send the request, once you send the request you will receive a string as a response.
  * URL: http://localhost:8090/home

## Screenshots
* register user request
![Screenshot (61)](https://github.com/rahljoshi/auth-assignment/assets/59885237/04299963-368f-40a0-a05f-d83b69bd8216)

* login user request
![Screenshot (62)](https://github.com/rahljoshi/auth-assignment/assets/59885237/e1e5a7b9-bd71-40db-8c6d-cfdf36967abc)

* authorized request
![Screenshot (63)](https://github.com/rahljoshi/auth-assignment/assets/59885237/b26137dc-6771-4496-9303-697f2e86125f)

* unauthorized request
![Screenshot (64)](https://github.com/rahljoshi/auth-assignment/assets/59885237/59b405ee-fe70-4bb0-9ff1-4906f468593b)
