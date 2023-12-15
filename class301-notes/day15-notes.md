# Read: Class 15

## What is OAuth

1. What is OAuth? OAuth (Open Authorization) is an open standard authorization protocol or framework designed to enable secure, delegated access to resources on behalf of a user. It allows unrelated servers and services to grant access to their assets without sharing the user's original credentials. OAuth is widely used for single sign-on (SSO) solutions across various websites and services.

2. Give an example of what using OAuth would look like. An example of using OAuth is when a user logs into a website and is given the option to sign in using credentials from another website or service. The user clicks on the option to log in with the second website, and the second website authenticates the user. The first website then obtains permission from the second website to access the user's information without requiring the user to enter separate login credentials.

3. How does OAuth work? What are the steps that it takes to authenticate the user?
User Initiates Action: The user initiates an action on one website that requires access to resources on another unrelated website.

Request for Access: The first website connects to the second website on behalf of the user, providing the user's verified identity.

Token Generation: The second website generates a one-time token and a one-time secret unique to the transaction.

Token Presentation: The first website gives this token and secret to the user's client software.

Authorization Provider: The client's software presents the token and secret to their authorization provider (which may or may not be the second site).

Authentication (if needed): If not authenticated, the client may be asked to authenticate. After authentication, the client approves the authorization transaction to the second website.

User Approval: The user approves a specific transaction type at the first website.

Access Token Issuance: The user is given an approved access token.

Token Exchange: The user gives the access token to the first website.

Resource Access: The first website gives the access token to the second website, allowing access to the user's resources.

Transaction Completion: The user sees a successfully completed transaction.

4. What is OpenID? OpenID is a related technology that focuses on authentication rather than authorization. It provides a way for users to log into multiple websites or services using a single identity, serving as a single sign-in solution. OpenID verifies the user's identity and vouches for it across different platforms. OpenID Connect, released in 2014, combines OpenID with OAuth to provide both authentication and authorization capabilities.

## Authroization and Authentication flows

1. What is the difference between authorization and authentication? Authentication: Authentication is the process of verifying the identity of a user, system, or application. It involves confirming that the credentials provided, such as a username and password, match the expected identity. Authentication establishes who you are.

Authorization: Authorization is the process of granting or denying access to specific resources or functionalities based on the authenticated user's permissions. Once authenticated, authorization determines what actions or data the user is allowed to access. Authorization defines what you are allowed to do.

2. What is Authorization Code Flow? The Authorization Code Flow is an OAuth 2.0 flow primarily designed for server-side applications. In this flow, the client (application) redirects the user to the authorization server, where the user logs in and grants permission. The authorization server then issues an authorization code that the client exchanges for an access token. This flow is suitable for secure, server-side applications where the client can keep its credentials confidential.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)? This is an extension of the Authorization Code Flow, specifically designed for mobile and native applications that may face additional security challenges. It uses a Proof Key for Code Exchange (PKCE) to protect against interception of the authorization code. PKCE adds a layer of security, especially in environments where it's challenging to securely store client secrets, as is common in mobile and single-page applications.

4. What is Implicit Flow with Form Post? The Implicit Flow is an alternative to the Authorization Code Flow, mainly intended for public clients (applications unable to securely store client secrets). While it's no longer considered best practice for obtaining access tokens, when used with Form Post response mode, it remains useful for obtaining an ID token for user authentication. This flow is commonly used in single-page applications (SPAs).

5. What is Client Credentials Flow? The Client Credentials Flow is designed for machine-to-machine (M2M) applications, such as CLIs, daemons, or backend services. In this flow, the system itself authenticates and authorizes the application, not a user. It is suitable for scenarios where typical user-based authentication methods are not applicable.

6. What is Device Authorization Flow?  This flow is used for input-constrained devices that connect to the internet. Instead of directly authenticating the user, the device asks the user to authorize it through a separate device. This is particularly useful for devices without a user-friendly input interface. The Device Authorization Flow is employed in mobile and native applications.

7. What is Resource Owner Password Flow? While not recommended, the Resource Owner Password Flow allows highly-trusted applications to request user credentials (username and password) directly, typically using an interactive form. This flow is used when other redirect-based flows, such as the Authorization Code Flow, cannot be employed. It is considered less secure and should be avoided unless necessary.

`## Things I want to know more about`
