AuthJs

AuthJs is a full-stack authentication system built with React for the frontend and Node.js (Express) for the backend. The project implements JSON Web Tokens (JWT) for secure authentication, MongoDB as the database, and React Router DOM for navigation between the /register, /login, and a secret page accessible via the / route. Additionally, custom error handling is integrated with React Toastify for a smooth user experience.

Table of Contents

1. Features

2. Tech stack

3. Usage

4. Folder structure

5. API endpoints



Features

1. User Registration

2. User Login

3. JWT-based Authentication

4. Secure access to a secret page

5. Custom error handling with React Toastify

Tech Stack


Frontend:

React: For building the user interface

React Router DOM: For client-side routing

React Toastify: For toast notifications (error handling)

Backend:

Node.js: Runtime environment for executing JavaScript on the server-side

Express: Web framework for building APIs

MongoDB: NoSQL database for storing user data

JWT: JSON Web Tokens for secure authentication


Usage:

Navigate to /register to create a new account.

After registration, navigate to /login to log in with your credentials.

Once logged in, you can access the secret page at /.

Register Page:

Users can create a new account by entering their email and password. The password is securely stored in the database.

<img width="1465" alt="Screenshot 2024-10-19 at 9 54 52 PM" src="https://github.com/user-attachments/assets/db698eef-ebea-431f-8b11-21f8e989d2b7">

Login Page:

Users can log in with their registered email and password. Upon successful login, a JWT is issued to authorize the user for accessing protected routes.

<img width="1467" alt="Screenshot 2024-10-19 at 10 23 52 PM" src="https://github.com/user-attachments/assets/c7e19234-f1fc-4946-bc44-6d2d559e4bfd">

Secret Page:

The secret page (/) is a protected route that can only be accessed by authenticated users.

<img width="1467" alt="Screenshot 2024-10-19 at 10 27 06 PM" src="https://github.com/user-attachments/assets/a64ec089-efc5-46f3-a9e8-ab56af01af8b">


Custom Error Handling:

Errors such as invalid login credentials or missing fields in forms are handled by React Toastify, which displays error messages to the user in a non-intrusive manner.


Folder Structure: 

<img width="711" alt="Screenshot 2024-10-19 at 11 00 17 PM" src="https://github.com/user-attachments/assets/492bc91f-20b9-4e86-bdfc-966e473969a4">

API Endpoints:

Register User:

<img width="711" alt="Screenshot 2024-10-19 at 11 07 58 PM" src="https://github.com/user-attachments/assets/4f19ebcb-c5a6-4770-8115-eaa8adeb6b0c">

-Request Body:

<img width="679" alt="Screenshot 2024-10-19 at 11 08 54 PM" src="https://github.com/user-attachments/assets/c75424bc-8eb0-411b-9caf-9a68d6bba441">

- Response: 201 Created on success, or error message.

Login User:

<img width="709" alt="Screenshot 2024-10-19 at 11 10 51 PM" src="https://github.com/user-attachments/assets/a2226284-0d49-41c5-ad71-02462006d034">

- Response: 200 OK and JWT token on success, or error message.

Secret Page (Protected)

<img width="707" alt="Screenshot 2024-10-19 at 11 12 05 PM" src="https://github.com/user-attachments/assets/fa236590-62e4-4c11-a5da-25b37857a16e">

- Requires Authorization header with a valid JWT token.








