# 🚕 Taxi service app

### 📄 Summary:
A simple web application that supports authentication, registration and CRUD operations and is built on Java Core technologies. The project follows an N-tier architecture and adheres to SOLID principles. It leverages Tomcat and MySQL technologies to facilitate seamless deployment and data storage. The app also gives the ability to connect cars with drivers, list all drivers, cars, and manufacturers, delete, update, and give the list of cars by driver login in each session.

### 💻 Project functionality:

- driver registration
- log in/out as driver
- display all drivers
- delete a driver
- add a manufacturer
- display all car manufacturers
- delete a manufacturer
- add a car
- display all cars
- delete a car
- add a driver to a car

### 🔨Technologies used
- Java 11
- JDBC
- JAVA Servlet API, JSTL, and JSP.
- MySql
- Tomcat, Maven

### 📂 Project structure:
The project follows an N-tier architecture and adheres to SOLID principles for optimal design and maintainability.

#### java/

- controller - HTTP servlets classes for processing requests
- dao - classes for CRUD operation with database
- exception - custom exceptions
- lib - custom implementation of field injector
- model - Car, Driver, Manufacturer models that used in service
- service - services for connection controllers and dao classes and perform business logic
- util - ConnectionUtil class to provide connection to database
- web.filter - authentication filter

#### resources/
- init_db.sql - file containing sql queries for creation a local copy of required database

#### webapp/
- WEB-INF - jsp pages and css files
- web.xml - mapping for servlets and endpoints

### How to run the project locally:
1. You will need JDK 11, tomcat 9.0.50 and mysql 8.0.
2. Clone the repository and execute queries from init_db.sql to create needed tables. 
3. Replace username, password and url in util/ConnectionUtil with your own.
4. Add a configuration of TomCat 9.0.50 to the project;
5. Run ```mvn package``` command in terminal and run Tomcat. 

