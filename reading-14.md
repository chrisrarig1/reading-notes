# Authentication

## What is OAuth

1. What is OAuth?

    - It is a open-standard authorization protocol. Secure, third party, user-agent, delegated authorization

2. Give an example of what using OAuth would look like.

    - When a website offers one or more opportunities to log on using another service like Google or Facebook

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    1. The first website connects to the second website on behalf of the user providing the user's verified identity

    2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved

    3. The first site sends the token and secret to the user's client software

    4. The client presents the secret and token to the authorization provider

    5. After authentication the client is asked to approve the authorization from the second site

    6. User approves and is given a approved access token to the first website

    7. The first website gives the access token to the second website as proof of auth

    8. The user is notified of the completed transaction and is given access to the website

4. What is OpenID?

    - Is used to identify that a human is accessing the website rather than a machine. It removes the need for a machine to authorize on behalf of a human.

## Authorization and Authentication Flows

1. What is the difference between authorization and authentication?

    - Authentication is the process of verifying who someone is and authorization is the process of verifying what specific items a user has access to

2. What is Authorization Code Flow?

    - The passing of an authorization code for a token. This must be server side due to the passing of the client secret as well.

3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

    - This is an additional security step in the Authorization Code Flow which introduces a secret called the Code Verifier

4. What is Implicit Flow with Form Post?

    - Intended for public clients. Has a streamlined workflow but does not securely store Client Secrets

5. What is Client Credentials Flow?

    - This is were the system authorizes and authenticates the app rather than the user

6. What is Device Authorization Flow?

    - This provides a link for the user to go to on another device to authenticate the device they are using

7. What is Resource Owner Password Flow?

    - For highly-trusted apps. This requires the users provide a username and password.

## Things I want to know more about

    - I am curious as to what we are going to use and how we will implement it

# Useful Links

- [What is OAuth](https://auth0.com/docs/authorization/flows)
- [Authorization and Authentication flows](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)