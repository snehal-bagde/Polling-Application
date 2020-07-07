# Polling-Application
      The aim of our project is to create a polls like social media application Twitter,
      YouTube. Where the User can create an account can make a public poll and also
      able to participate (Vote) any public poll.
      This application is build by using Spring Boot, ReactJs where we used Spring
      Security along with JWT Authentication and MySQL database for storage



Steps to Setup the Spring Boot Back end app (polls) 

1. Clone the application 

      git clone https://github.com/snehal-bagde/Polling-Application.git 
      cd polls 

2. Create MySQL database 

      create database polling_app 

 
3. Change MySQL username and password as per your MySQL installation 

      open src/main/resources/application.properties file. 
      change spring.datasource.username and spring.datasource.password properties as per your mysql installation 

  
4. Run the app 

      Run the spring boot app using IDE 
      The server will start on port 8080. 

  
5. Default Roles 

      The spring boot app uses role based authorization powered by spring security. To add the default roles in the database use below queries, 
      INSERT INTO `roles` (`id`, `name`) VALUES (1, 'ROLE_USER'); 
      INSERT INTO `roles` (`id`, `name`) VALUES (2, 'ROLE_ADMIN'); 

      Any new user who signs up to the app is assigned the ROLE_USER by default. 

  

Steps to Setup the React Front end app (polling-app-client) 

      First go to the polling-app-client folder - 

      cd polling-app-client 

      Then type the following command to install the dependencies and start the application  

      npm install && npm start 

      The front-end server will start on port 3000. 
