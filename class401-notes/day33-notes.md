# Read: Class 33

1. **What is the primary purpose of JSON Web Tokens (JWTs) and how do they work in terms of encoding and decoding data?**

Purpose: JSON Web Tokens are a standard for representing claims between two parties. In Django, JWTs are often used for authentication and authorization purposes. They allow the server to encode information in a compact and self-contained manner, which can be transmitted between parties. JWTs are commonly used for token-based authentication.

Encoding and Decoding: JWTs consist of three parts: a header, a payload, and a signature. The header and payload are JSON objects encoded as Base64 strings. The header typically contains the algorithm used for the signature, and the payload contains the claims. The server signs the JWT with a secret key, and the client can decode the token to read the claims. This allows for stateless authentication as the server doesn't need to store session information.

2. **How does JWT Authentication integrate with Django REST Framework to secure API endpoints, and what are the key components involved in this process?**

Integration: Django REST Framework (DRF) supports JWT authentication out of the box. To integrate JWT authentication into a Django application, you can use third-party packages like djangorestframework-simplejwt or djangorestframework-jwt. These packages provide views and serializers for handling JWT-based authentication.

Key Components:

Views: DRF provides views like ObtainTokenView for token generation and TokenVerifyView for token verification.

Serializers: Serializers handle the conversion between JSON data and Python objects. DRF provides serializers for handling JWT-related data.

Middleware: Middleware can be used to check the JWT in incoming requests and authenticate users accordingly.

3. **Why is Django’s built-in runserver not suitable for production environments, and what are some alternative server options that should be considered for deploying a Django application?**

Limitations of runserver: The built-in runserver command in Django is convenient for development but is not suitable for production. It lacks features like performance optimizations, security measures, and robustness required for a production environment. It's not designed to handle high loads and does not provide necessary security features.

Alternative Server Options:

Gunicorn (Green Unicorn): Gunicorn is a popular choice for deploying Django applications. It can handle multiple worker processes, providing better concurrency and performance.

uWSGI: Another option for serving Django applications is uWSGI, which is a fast and flexible application server.
nginx or Apache: While not application servers, these web servers are often used as reverse proxies in conjunction with Gunicorn or uWSGI to improve performance and handle tasks like SSL termination.

Deployment Platforms: Platforms like Heroku, AWS Elastic Beanstalk, and Docker can also simplify the deployment process and provide additional tools for scaling and managing Django applications in production.

## `Things I want to know more about`
