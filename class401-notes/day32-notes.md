# Read: Class 32

1. **What are the key components and purpose of Django Rest Framework (DRF) permissions, and how do they help in securing an API?**

Key Components and Purpose: DRF permissions are a crucial part of securing APIs built using Django Rest Framework. They provide a way to control access to different parts of the API. The key components include:

Permission classes: These are classes that determine the allowable actions for a user. Examples include IsAuthenticated, IsAdminUser, and custom permission classes.

Authentication classes: These are classes that determine how the user is authenticated. Examples include SessionAuthentication and TokenAuthentication.

Permission checks: DRF uses permission checks to determine if a user has the necessary permissions to perform a specific action on a resource.

Purpose: DRF permissions help in enforcing security measures by controlling access to API endpoints based on user authentication and authorization. They ensure that only authorized users can perform certain actions, such as creating, updating, or deleting resources.

2. **In SQL, what is the purpose of the SELECT statement, and how would you use it to retrieve all columns from a table called ‘employees’?**

Purpose: The `SELECT` statement in SQL is used to retrieve data from one or more tables. It is the fundamental query statement that allows you to fetch specific columns or all columns from a table, apply conditions, and more.

3. **Can you explain the role of DRF Generic Views and provide examples of their usage in building a RESTful API?**

Role: DRF Generic Views are pre-built views provided by Django Rest Framework that simplify the implementation of common patterns in API development. They abstract away much of the boilerplate code and provide a consistent interface for performing CRUD (Create, Retrieve, Update, Delete) operations.

Example:

`from rest_framework.generics import ListAPIView`
`from .models import YourModel`
`from .serializers import YourModelSerializer`

`class YourModelListView(ListAPIView):`
    `queryset = YourModel.objects.all()`
    `serializer_class = YourModelSerializer`

## `Things I want to know more about`
