# Read: Class 31

1. **What are the key components of a Docker container, and how do they help streamline the development and deployment of applications?**

Docker containers consist of the following key components:

Docker Image: A lightweight, standalone, and executable package that includes everything needed to run a piece of software, including the code, runtime, libraries, and system tools.

Container: An instance of a Docker image. It runs the application in an isolated environment, ensuring consistency across different environments (development, testing, production).

Dockerfile: A script that contains instructions to build a Docker image. It specifies the base image, sets up the environment, installs dependencies, and configures the application.

Docker helps streamline development and deployment in several ways:

Consistency: Ensures that the application runs the same way in any environment.

Isolation: Each container encapsulates the application and its dependencies, avoiding conflicts with the host system.

Portability: Containers can run on any system supporting Docker, making it easier to deploy applications across different environments.

Resource Efficiency: Containers share the host OS kernel, which reduces overhead compared to traditional virtual machines.

2. **Describe the primary steps involved in building a library website using Django, including essential components like models, views, and templates.**

Building a library website in Django involves several steps:

Models: Define models to represent entities such as books, authors, and categories. Use relationships (e.g., ForeignKey) to establish connections between models.

Views: Create views to handle user requests and interact with the models. Views retrieve data from the database and pass it to templates for rendering.

Templates: Design HTML templates to display information. Templates use Django template language to dynamically render content.

URLs: Configure URL patterns in the urls.py file to map URLs to specific views.

Static Files: Manage static files (CSS, JS) for styling and interactivity.

Forms: Implement forms for user input, such as searching for books or submitting reviews.

Authentication and Authorization: Implement user authentication for features like borrowing books. Ensure proper authorization to restrict access to certain views.

Admin Interface: Utilize Django's admin interface for managing library data.

3. **Can you explain the primary differences between Django and Django REST framework?**

Django:

Purpose: Primarily designed for building web applications.

Functionality: Provides a full-stack framework with built-in features for templates, ORM, authentication, and more.

Output Format: Outputs HTML pages for browser rendering.

View Functionality: Views handle rendering HTML pages and processing form submissions.

Django REST framework (DRF):

Purpose: Specialized for building Web APIs.

Functionality: Extends Django to support RESTful API development.

Output Format: Outputs data in various formats such as JSON or XML.

View Functionality: Uses serializers and views for processing and presenting data, often with class-based views for API endpoints.

In summary, Django is a full-stack web framework, while Django REST framework is an extension that focuses specifically on building RESTful APIs.

## `Things I want to know more about`
