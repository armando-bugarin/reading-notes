# Read: Class 29

1. **What are the key benefits of using a Django Custom User Model, and how does it differ from the default Django User Model?**

Flexibility: A custom user model allows you to define your own fields, providing flexibility to tailor the user model to your specific project needs.

Scalability: You can add or remove fields without any constraints, ensuring scalability as your project evolves.

Consistency: By using your own user model, you can maintain consistency with the rest of your data models, creating a unified and organized database structure.

Compatibility: It allows for seamless integration with third-party packages and libraries that might depend on a custom user model.

Differences from Default User Model:

The default User model includes predefined fields like username, email, and password. A custom model lets you define these fields according to your project requirements.

If you need additional fields like profile_picture, date_of_birth, etc., a custom model allows you to include them easily.

2. **Explain the process of creating and implementing a Custom User Model in Django, including the necessary changes to settings.py and the required model fields.**

a. Define the Custom Model:

In your Django app, create a new model that extends AbstractUser from django.contrib.auth.models.

Define the fields you want in your custom user model within this class. For example, you might want to include additional fields such as email, profile_picture, etc.

b. Update settings.py:

In your project's settings.py file, add a reference to your custom user model using the AUTH_USER_MODEL setting.

Set AUTH_USER_MODEL to the path of your custom user model, typically in the format 'your_app.CustomUser'.

3. **What is DjangoX and how does it complement or extend the functionality of Django? Provide an example use case for incorporating DjangoX in a project.**

Description:

DjangoX is not a specific package or library. It might be a reference to projects, tools, or frameworks built on top of Django to enhance its functionality.

Example Use Case:

Suppose you are working on a project that requires additional features such as user authentication, user profiles, and user management. Instead of building everything from scratch, you could use DjangoX, which might provide pre-built components, templates, or views for common functionalities. This can save development time and ensure best practices in implementing features like authentication, profiles, and permissions.

## `Things I want to know more about`
