# Read: Class 34

1. **What are the key principles to follow when organizing and configuring Django settings for a project, according to the “Django Settings Best Practices” reading?**

Keep settings in a separate module: Group your settings in a separate module (usually named settings.py) to maintain a clean and organized structure.

Use environment variables: Avoid hardcoding sensitive information like secret keys or database passwords directly in your settings. Instead, use environment variables to keep this information secure and customizable.

Split settings into different files: Divide your settings into separate files based on functionality (e.g., base.py, development.py, production.py) to make it easier to manage and understand.

Use local_settings.py for local development: Create a local_settings.py file for local development settings that can override default settings for debugging or testing purposes.

Use default settings wisely: Leverage Django's default settings whenever possible, and only override what's necessary. This helps maintain compatibility with third-party apps and future Django updates.

2. **How does the White Noise library contribute to the efficient serving of static files in a Django application, and what are the steps to integrate it into a project?**

Purpose: White Noise is a Python library for serving static files efficiently in a Django application, particularly in production environments. It helps reduce the need for a separate web server (like Nginx or Apache) to handle static files.

Integration Steps:

Install White Noise: pip install whitenoise

Add whitenoise.middleware.WhiteNoiseMiddleware to the MIDDLEWARE setting in your settings.py.

Configure STATIC_URL and STATICFILES_STORAGE in your settings.py. Set STATICFILES_STORAGE to 'whitenoise.storage.CompressedManifestStaticFilesStorage'.

Make sure whitenoise is included in your requirements.txt or Pipfile if you're using pipenv.

Ensure your application is ready to serve static files.

3. **What is the purpose of Cross-Origin Resource Sharing (CORS) in web applications, and how can it be implemented and configured in a Django project to control access to resources?**

Purpose: CORS is a security feature implemented by web browsers to control which web pages can access resources on a given domain. It prevents unauthorized cross-origin requests that could lead to security vulnerabilities.

Implementation in Django:

Install django-cors-headers: pip install django-cors-headers

Add 'corsheaders.middleware.CorsMiddleware' to the MIDDLEWARE setting in your settings.py.
Add 'corsheaders' to the INSTALLED_APPS setting.

Configure CORS_ALLOWED_ORIGINS to specify which origins are allowed to access your resources. This can be a list of allowed domains or '*' to allow any domain (not recommended for production).

Optionally, you can customize other settings like CORS_ALLOW_METHODS and CORS_ALLOW_HEADERS based on your application's requirements.

## `Things I want to know more about`
