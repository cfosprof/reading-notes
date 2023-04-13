# Class 12

## Readings: CRUD

<details markdown="block"><summary>Things</summary>

### 1. In your own words, describe what each group of status code represents: 

100’s = Informal responses, indicating the request has been received and the process is continuing.
200’s = Success codes, inicating the request was successfully accepted, but not necessariyl processed.
300’s = Redirection codes, indicating the client must take some additional action in order to complete their request.
400’s = Client error codes, indicating the request was not successfully received, often due to invalid syntax or headers.
500’s = Server error codes, indicating the server failed to fulfill an apparently valid request. These codes are often used when the server is overloaded or there is an error in the server itself.



### 2. What is a status code 202?

Accepted - The request has been accepted for processing, but the processing has not been completed. The request might or might not be eventually acted upon, and may be disallowed when processing occurs.

### 3. What is a status code 308?

Permanent redirect - This and all future requests should be directed to the given URI.

### 4. What code would you use if an update didn’t return data to a client?

204 - No Content - The server successfully processed the request and is not returning any content.

### 5. What code would you use if a resource used to exist but no longer does?

410 - Gone - Indicates that the resource requested is no longer available and will not be available again. 

### 6. What is the ‘Forbidden’ status code?

403 - Forbidden - The client does not have access rights to the content; that is, it is unauthorized, so the server is refusing to give the requested resource. Unlike 401, the client's identity is known to the server.

### 9. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

To keep our database secure and to keep our database string private.

### 10. What is middleware?

Middleware is software that provides common services and capabilities to applications outside of what's offered by the operating system.

### 11. What does app.use(express.json()) do?

It parses incoming requests with JSON payloads and is based on body-parser. 

### 12. What does the /:id mean in a route?

It is a parameter that is passed to the route. It is a variable that can be used to access the data in the database.

### 13. What is the difference between PUT and PATCH?

PUT is used to update a resource, and PATCH is used to update a resource partially.

### 14. How do you make a default value in a schema?

You can use the default property in the schema. 

### 15. What does a 500 error status code mean?

Internal Server Error - The server has encountered a situation it doesn't know how to handle.

### 16. What is the difference between a status 200 and a status 201?

200 tells the client that the request was successful. 201 tells the client that the request was successful and a resource has been created.

</details>