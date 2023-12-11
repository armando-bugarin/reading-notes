# Read: Class 12

## Status Codes Based on REST Methods

1. **In your own words, describe what each group of status code represents:**

100’s = These codes inform the client that the header part of the request has been received, and the server will try to comply with the client's transmission demand. They are about setting up the communication and may indicate that the client's request will fail.

200’s = These codes indicate that the client's request was accepted and processed successfully. They signify that the requested action was completed without errors.

300’s = These codes inform the client that the resource they are requesting is not available at the expected location anymore. The client needs to issue a request to the new location.

400’s = These codes indicate that there was an issue with the client's request. It could be due to invalid input, missing authentication, or other client-side errors. The client should confirm the input parameters before retrying the request.

500’s = These codes indicate problems on the server-side. They may be temporary or permanent, and the client is often advised to retry the same request.

2. **What is a status code 202?** It is used to indicate that the request was valid, but its processing will finish sometime in the future. It is often used for asynchronous processing.

3. **What is a status code 308?** It is a permanent redirect status code. It tells the client to use another URL to access the resource and not use the current URL anymore.

4. **What code would you use if an update didn’t return data to a client?** Status code 204 (No Content) is recommended for updates that don't return data to the client.

5. **What code would you use if a resource used to exist but no longer does?** Status code 410 (Gone) is recommended for cases where a resource used to exist but got deleted or moved.

6. **What is the ‘Forbidden’ status code?** Status code 403 (Forbidden) is clients not having permissions to access a resource.

## Build A REST API With Node.js, Express, & MongoDB - Quick

1. **Why do we need to pull our MongoDB database string out of our server and put it into our .env?** To secure sensitive info like DB connection strings, keeping them in a separate .env file adds privacy and avoids unintentional exposure.

2. **What is middleware?** Middleware are functions in web development that handle HTTP request and response objects. They add functionality, such as authentication or logging, to the application.

3. **What does `app.use(express.json())` do?** This Express middleware parses incoming JSON payloads in request bodies, enabling the server to work with JSON data.

4. **What does the `/:id` mean in a route?** It indicates that the route will accept an id parameter.

5. **What is the difference between `PUT` and `PATCH`?** PUT is used to replace the entire resource, while PATCH is used to update a specific part of the resource.

6. **How do you make a default value in a schema?** In a schema, use the default property to set default values for fields.

7. **What does a `500` error status code mean?** Signifies an unexpected server error, indicating the server's inability to fulfill the request.

8. **What is the difference between a status `200` and a status `201`?** A status 200 is a successful response, while a status 201 is a successful response that also created a new resource.

`## Things I want to know more about`
