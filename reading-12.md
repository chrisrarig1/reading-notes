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

## Things I want to know more about

- I am wondering if these codes will be implemented the same way we have been throwing errors in our code already.

# Useful Links

- [Status Codes](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)