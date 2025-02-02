# Authorization and Authentication

## Objective

In this assignment, you will continue to enhance your REST API application from the [previous task](https://github.com/AM1007/goit-pythonweb-hw-08).

## Technical Requirements

- Implement an authentication mechanism in your application.
- Implement authorization using JWT tokens, ensuring that all operations with contacts are performed only by registered users.
- Users should only have access to their own contacts and operations.
- Implement a mechanism for verifying the email address of registered users.
- Limit the number of requests to the /me route.
- Enable CORS for your REST API.
- Add functionality for users to update their avatar (use the Cloudinary service for this feature).

## Additional Specifications

1.  During registration, if a user with the provided `email` already exists, the server should return an `HTTP 409 Conflict` error.
2.  The server must hash passwords and never store them in plain text in the database.
3.  Upon successful user registration, the server should respond with an `HTTP 201 Created` status and include the new user’s data.
4.  For all `POST` operations (creating new resources), the server must return an `HTTP 201 Created` status.
5.  For POST requests requiring user authentication, the server should accept the user’s credentials (username and password) in the request body.
6.  If the user does not exist or the password is incorrect, the server should return an `HTTP 401 Unauthorized` error.
7.  Authorization using `JWT` tokens must be implemented through an `access_token`.
8.  All environment variables must be stored in a `.env` file. Sensitive data should not be hardcoded directly in the code.
9.  Use Docker Compose to run all services and databases in the application.
