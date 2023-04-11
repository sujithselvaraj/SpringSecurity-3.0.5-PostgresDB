# SpringSecurity-3.0.5-PostgresDB

To create a project go the https://start.spring.io website

Dont forget to create a postgres database

Here i am using postgres and my database name is jwt_security


Refer to the application.yml for connecting the application and the database.
Refer the pom.xml file for the dependencies used in our project.


use https://www.allkeysgenerator.com for generating the encryption secret key in JwtService ...here i used to create the key in 256 bits


After completing the project go and hit the post man with

http://localhost:8080/api/v1/auth/register with post request and with your own body as a json format to generate token


sample json:
{
    "firstname":"sujith",
    "lastname":"selva",
    "email":"sujith@gmail.com",
    "password":"1234"
} 


http://localhost:8080/api/v1/auth/authenticate with post request with the body of same email and password given and generate authtoken

{
    "email":"sujith@gmail.com",
    "password":"1234"
}

After that hit http://localhost:8080/api/v1/demo with get request with authorization of bearer token with the authtoken




