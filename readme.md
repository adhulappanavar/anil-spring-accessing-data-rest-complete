Reference - https://spring.io/guides/gs/accessing-data-rest/

Commnad Line usage

1) Build and Package
$mvn package

2) Execute the spring project from command line
$mvn spring-boot:run


3) Test from Browser
open 
http://localhost:8080

http://localhost:8080/people

4) Adding a person using postman
Method : POST
URL : http://localhost:8080/people
Content-Type:application/json
Body : {  "firstName" : "Frodo",  "lastName" : "Baggins" }

5) Adding person using CURL
$ curl -i -X POST -H "Content-Type:application/json" -d "{  \"firstName\" : \"Frodo\",  \"lastName\" : \"Baggins\" }" http://localhost:8080/people
HTTP/1.1 201 Created
Server: Apache-Coyote/1.1
Location: http://localhost:8080/people/1
Content-Length: 0
Date: Wed, 26 Feb 2014 20:26:55 GMT