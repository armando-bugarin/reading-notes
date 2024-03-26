# Read: Class 41

1. **Explain the concept of dynamic routes in Next.js and how they differ from static routes.**

Dynamic routes in Next.js allow you to create pages with variable paths. This means you can create pages that can match different route patterns based on the parameters provided. For example, if you have a page for blog posts, you might want to create a dynamic route to handle different post slugs.

Static routes, on the other hand, are pre-rendered at build time and don't depend on external data. Dynamic routes are useful when you have pages that depend on data that can change, like fetching content from an API.

2. **Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use?**

The process of deploying a Next.js application typically involves the following steps:

Build the Application: Use the next build command to create a production-ready build of your Next.js application.

Choose a Hosting Platform: There are various hosting platforms where you can deploy your Next.js app. Some popular options include Vercel, Netlify, AWS, and Heroku.

Configure Deployment Settings: Different platforms may have different configuration steps. For example, Vercel often auto-detects Next.js projects, while on AWS, you might need to configure serverless functions.

Deploy: Once configured, trigger the deployment process on your chosen platform. The platform will take care of deploying your application.

3. **How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application.**

Next.js automatically serves static files under the public directory in the root of your project. Next.js will handle the correct path resolution for you. Remember that anything inside public is served at the root level of your website.

This approach is useful for assets that don't need to go through the build process, like images, fonts, or other static files. For assets that require processing (e.g., stylesheets), you should import them in your JavaScript/TypeScript files so they can be optimized during the build.

## `Things I want to know more about`
