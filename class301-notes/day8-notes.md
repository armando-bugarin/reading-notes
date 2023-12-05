# Read: Class 08

## API Design Best Practices

1. **What does REST stand for?** Representational State Transfer

2. **REST APIs are designed around a ____.** Designed around resources

3. **What is an identifier of a resource? Give an example.** A URI (Uniform Resource Locator) that identifies that resource

4. **What are the most common HTTP verbs?** GET, POST, PUT, PATCH, and DELETE

5. **What should the URIs be based on?** concept of resources

6. **Give an example of a good URI.** GET /blog/posts/1

7. **What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?** It is a bad thing. It is when you impose a lot of data on a web server; expose a large number of small resources

8. **What status code does a successful GET request return?** HTTP status code 200

9. **What status code does an unsuccessful GET request return?** 404 if the resource not found. 204 if found but no response body included in HTTP response

10. **What status code does a successful POST request return?** HTTP status code 201

11. **What status code does a successful DELETE request return?** HTTP status code 204

`## Things I want to know more about`
