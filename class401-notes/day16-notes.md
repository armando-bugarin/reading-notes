# Read: Class 16

1. **What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?**

Key Characteristics:

Event-Driven: Serverless computing is triggered by events, such as HTTP requests, database updates, or file uploads.

No Server Management: Developers don't need to worry about server provisioning, scaling, or maintenance.

Scalability: Automatically scales based on demand, handling varying workloads efficiently.

Pay-as-You-Go Pricing: Users are billed based on the actual resources consumed during the execution of functions.

Stateless: Functions are designed to be stateless, and each function execution is independent.

Difference from Traditional Server-Based Architectures:

In traditional server-based architectures, you manage and maintain servers, ensuring they are provisioned, scaled, and updated. In serverless, these concerns are abstracted away.

Serverless is more cost-effective as you only pay for actual usage, while traditional servers may involve fixed costs.

Serverless encourages a microservices architecture, breaking down applications into smaller, independently deployable functions.

2. **How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?**

Getting Started:

Sign Up: Create an account on Vercel.

Install CLI: Install Vercel CLI using `npm install -g vercel`.

Login: Run vercel login to log in using your Vercel account.

Deploying Serverless Function:

Create a Function: Create a directory with your serverless function (e.g., api/myfunction.js).

Deploy: Run `vercel --prod` in the project directory.

Access URL: Vercel provides a URL for your function (e.g., https://your-project.vercel.app/api/myfunction).

3. **What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?**

APIs (Application Programming Interfaces):

APIs define how software components should interact, allowing applications to communicate with external services or libraries.

In Python, you can use libraries like requests to make HTTP requests to APIs.

4. **What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?**

`requests` is a popular Python library for making HTTP requests.

## `Things I want to know more about`
