# User Authentication and Registration System 

This project is a Spring Boot application that implements a user authentication and registration system. It provides functionality for users to register, login, and logout, with server-side validations and session management.

## Objectives

- Implement user registration with server-side validations for fields like username, email, password, and additional form elements.
- Enable user login with authentication against stored credentials (hashed passwords).
- Manage user sessions to keep users authenticated across multiple requests until they logout.
- Implement logout functionality to clear the user's session.

## Technologies Used

- **Spring Boot**: For creating the application and managing dependencies.
- **Spring MVC**: For handling web requests and responses.
- **Spring Data JPA**: For database operations and entity management.
- **Thymeleaf**: For server-side templating and rendering HTML pages.
- **MySQL**: As the database for storing user information.
- **BCrypt**: For hashing passwords securely.
- **Java 11**: Programming language used for backend logic.

## Usage

1. **Registration**
   - Navigate to `/register` to access the registration form.
   - Fill out the required fields (username, email, password, etc.) and submit the form.
   - Server-side validations will ensure data integrity, such as checking for valid email format and password requirements.

2. **Login**
   - Navigate to `/login` to access the login form.
   - Enter valid credentials (email and password) to authenticate and start a session.
   - Invalid credentials will prompt error messages based on server-side validations.

3. **Logout**
   - Click on the logout button or link available in the application to invalidate the current session.
   - After logout, attempting to access protected pages like `/success` should redirect you back to the login page.

4. **Success Page**
   - After successful login, navigate to `/success`.
   - This page should display a welcome message or user-specific information.
   - Trying to access `/success` after logout should redirect you to the login page to reauthenticate.
