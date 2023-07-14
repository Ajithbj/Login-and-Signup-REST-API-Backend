# Login-and-Signup-REST-API-Backend

Installation and Setup:

Clone the repository to your local machine.
Ensure you have Java JDK (version 8 or higher) installed.
Install Maven or Gradle as the build tool.
Open the project in your preferred IDE.

Configuration:

Configure the database connection properties in the application.properties file located in the src/main/resources directory.
Make sure the H2 database dependency is included in the project's pom.xml or build. gradle file.

Database Schema:

The project utilizes the H2 database for storing user account information. The database schema consists of a users table with the following fields:

id: Unique identifier for each user.
username: User's username.
password: Hashed and salted password.
email: User's email address.
Additional fields as per your project requirements.

Endpoints:

The REST API provides the following endpoints:

/api/signup (POST): Allows users to create a new account. Accepts JSON payload with user details and stores them securely in the database.
/api/login (POST): Verifies user credentials and generates a web token upon successful authentication. Accepts JSON payload with login credentials.
/api/hello (GET): Returns a "Hello from GreenStitch" message. Requires authentication using the generated web token.
Security and Web Tokens
The project implements security measures to protect user data and prevent unauthorized access. It utilizes JSON Web Tokens (JWT) for user authentication and authorization. The token is generated upon successful login and must be included in the Authorization header of subsequent requests to access protected resources.

Error Handling and Validation:

The project incorporates error handling and input validation to ensure data integrity and provide meaningful error messages to clients. Proper exception handling is implemented throughout the application.

Dependencies:

The project relies on the following libraries and frameworks:

Spring Boot: Provides the foundation for the backend application.
Spring Security: Implements authentication and authorization mechanisms.
H2 Database: Handles the storage and retrieval of user account information.
JWT (JSON Web Tokens): Enables secure authentication and authorization.
Make sure to include the necessary dependencies in your project's pom.xml or build.gradle file.

Testing:

To test the API endpoints, you can use tools like cURL, Postman, or any REST client of your choice. Make sure to include the required headers and payload as mentioned in the API documentation.

output:


![Screenshot (26)](https://github.com/Ajithbj/Login-and-Signup-REST-API-Backend/assets/88621660/185677dc-2100-465d-b0de-a19858d4dcab)
![Screenshot (27)](https://github.com/Ajithbj/Login-and-Signup-REST-API-Backend/assets/88621660/ed69eb1e-fad6-40cb-b3c2-c32b907664fc)
![Screenshot (28)](https://github.com/Ajithbj/Login-and-Signup-REST-API-Backend/assets/88621660/4b56c76d-0e12-4052-8045-35bb59a9d7d4)
