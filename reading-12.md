# CRUD

1. In your own words, describe what each group of status code represents:
   - 100’s = Request received and the server will try, but don't get your hopes up
   - 200’s = Successful in sending
   - 300’s = Request not found at location
   - 400’s = Request is incorrect or invalid
   - 500’s = Server threw an error...possibly busy server

2. What is a status code 202?

    - Used in **Async** processing and tells the client that the request is valid.

3. What is a status code 308?

    - This notifies the user to use another URL and that the request is no longer available at this address

4. What code would you use if an update didn’t return data to a client?

    - Code 204

5. What code would you use if a resource used to exist but no longer does?

    - 410 Gone

6. What is the ‘Forbidden’ status code?

    - 403 - No permission

# Rest API

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

    - Because when we deploy we will want to use something other than our local server

2. What is middleware?

    - Code that runs when a server gets a request but before its passed to the route

3. What does app.use(express.json()) do?

    - Allows the server to accept json

4. What does the /:id mean in a route?

    - It is a parameter.

5. What is the difference beween PUT and PATCH?

    - Patch only updates what the user passes
    - Put updates all the information

6. How do you make a default value in a schema?

    - By typing default:

7. What does a 500 error status code mean?

    - Internal server error

8. What is the difference between a status 200 and a status 201?

    - 200: Request was received and understood and is being processed
    - 201: Request was successful and resulted in a resource being created

## Things I want to know more about

- I am wondering if these codes will be implemented the same way we have been throwing errors in our code already.

# Useful Links

- [Status Codes](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
- [REST](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)