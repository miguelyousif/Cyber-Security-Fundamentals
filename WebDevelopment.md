# Web Development

**HTTP Requests and Responses**

*Answer the following questions about the HTTP request and response process.*

1. What type of architecture does the HTTP request and response process occur in?
- Client-Server Architecture

2. What are the different parts of an HTTP request?
- Request Line, Request Headers and Request Body

3. Which part of an HTTP request is optional?
- Request Body

4. What are the three parts of an HTTP response?
- Headers, Status Line, Body

5. Which number class of status codes represents errors?
- 400s Range

6. What are the two most common request methods that a security professional will encounter?
- GET and POST requests

7. Which type of HTTP request method is used for sending data?
- POST Request

8. Which part of an HTTP request contains the data being sent to the server?
- Request body

9. In which part of an HTTP response does the browser receive the web code to generate and style a web page?
- Response body

**Using curl**

*Answer the following questions about curl:*

10. What are the advantages of using curl over the browser?
- The ability to manage HTTP Requests/Responses in a repetitive, programmatic way.
- You can quickly test HTTP Requests in ways that can be automated.
- It allows the ability to make adjustments as needed.
- The ability to support numerous protocols even if a UI is not present.

11. Which curl option is used to change the request method?
- -X

12. Which curl option is used to set request headers?
- -H

13. Which curl option is used to view the response header?
- -I

14. Which request method might an attacker use to figure out which HTTP requests an HTTP server will accept?
- Options

**Sessions and Cookies**

*Recall that HTTP servers need to be able to recognize clients from one another. They do this through sessions and cookies.
Answer the following questions about sessions and cookies:*

![Capture 1](https://user-images.githubusercontent.com/94030092/159802387-27541871-2642-4fe5-9401-32b1bf452f9b.PNG)

15. Which response header sends a cookie to the client?
- Set-Cookie HTTP

![Capture 2](https://user-images.githubusercontent.com/94030092/159802633-121f467f-63c3-4659-9f2a-6a1decb31a0e.PNG)

16. Which request header will continue the client's session?
- HTTP keep-alive

**Example HTTP Requests and Responses**

*Look through the following example HTTP request and response and answer the following questions:*

**HTTP Request**

![Capture 3](https://user-images.githubusercontent.com/94030092/159802798-4c67c49e-2c78-4487-b0c4-f295d5b86abf.PNG)

17. What is the request method?
- POST

18. Which header expresses the client's preference for an encrypted response?
- Upgrade-Insecure-Requests

19. Does the request have a user session associated with it?
- No, the session is not yet reestablished.

20. What kind of data is being sent from this request body?
- Login Credentials (username=Barbara&password=password)

**HTTP Response**

![Capture 4](https://user-images.githubusercontent.com/94030092/159803101-ed95a452-d12b-4a78-a9f2-56221cf5e67d.PNG)

21. What is the response status code?
- 200

22. What web server is handling this HTTP response?
- Apache webserver

23. Does this response have a user session associated to it?
- Yes, SessionID=5

24. What kind of content is likely to be in the [page content] response body?
- Detail of page configuration.

25. If your class covered security headers, what security request headers have been included?
- Strict-Transport-Security: max-age=31536000; includeSubDomains

**Monoliths and Microservices**

*Answer the following questions about monoliths and microservices:*

26. What are the individual components of microservices called?
- Services

27. What is a service that writes to a database and communicates to other services?
- APIs

28. What type of underlying technology allows for microservices to become scalable and have redundancy?
- Load Balancer Technology

**Deploying and Testing a Container Set**

*Answer the following questions about multi-container deployment:*

29. What tool can be used to deploy multiple containers at once?
- Docker

30. What kind of file format is required for us to deploy a container set?
- .yml; YAML format

**Databases**

31. Which type of SQL query would we use to see all of the information within a table called customers?
- SELECT column_name FROM customers;

32. Which type of SQL query would we use to enter new data into a table? (You don't need a full query, just the first part of the statement.)
- INSERT INTO table_name (column_1, column_2, column_3) VALUES (value_1, ‘value_2’, value_3);

33. Why would we never run DELETE FROM <table-name>; by itself?
- It would delete the entire table, there is no select statement.
