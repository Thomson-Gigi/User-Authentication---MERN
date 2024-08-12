
#User Authentication System - MERN

This project is a user authentication system built using the MERN stack (MongoDB, Express.js, React.js, Node.js). It allows users to register, log in, and log out, with an additional profile page that only logged-in users can access.

Features
User Registration: Users can create an account by providing a username, email, and password. The system includes basic form validation to ensure that no fields are empty and that the email format is valid. Passwords are securely hashed before they are stored in the database, ensuring that user data is protected.

User Login: Users can log in using their email and password. The system uses session-based authentication to manage user sessions, meaning that once a user is logged in, their session remains active until they log out or the session expires. This helps to manage access to protected routes and pages.

User Profile Page: After logging in, users are redirected to a simple profile page where they can view their username and email. This page is protected and only accessible to users who are currently logged in, ensuring that sensitive information is not exposed to unauthorized users.

Logout Functionality: Users have the option to log out, which effectively ends their session. This is important for maintaining security, especially on shared devices, as it prevents others from accessing the logged-in user's account.

Installation
The project requires Node.js, npm, and MongoDB to be installed on your system. After cloning the repository, you need to install dependencies for both the backend and frontend parts of the application. The backend server handles the API and database interactions, while the frontend handles user interactions through a React-based interface.

You will need to configure environment variables, such as the MongoDB connection string and a secret key for session management. Once set up, you can run the backend and frontend servers concurrently, allowing the application to function.

Project Structure
Backend:
Server Setup: The backend is set up using Node.js and Express.js. The server is configured to handle API routes, including user registration, login, and logout.
Database: MongoDB is used as the database, with Mongoose managing schemas and models for user data.
Authentication: User sessions are managed using session-based authentication. Passwords are hashed using bcrypt.js for security.
Frontend:
React Components: The frontend is built with React.js, and includes components for registration, login, and the user profile page.
Routing: React Router is used for navigating between pages. Protected routes are implemented to ensure that only authenticated users can access certain pages.
Form Handling: Forms for registration and login are responsive, with validation to ensure correct data entry. Errors are properly handled and displayed to the user.
Key Components
Server.js: The entry point for the backend server.
Models: Contains Mongoose models for managing user data.
Routes: Defines the API endpoints for user actions like registration and login.
React Components: Includes components for handling user input, displaying data, and managing navigation between pages.
Technologies Used
Frontend:

React.js for building the user interface.
React Router for managing navigation.
Axios for making API requests to the backend.
Backend:

Node.js and Express.js for building the API and managing server-side logic.
MongoDB and Mongoose for data storage and management.
bcrypt.js for secure password hashing.
jsonwebtoken for handling session-based authentication.
