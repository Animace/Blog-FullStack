# Blog App Features

This document outlines the key features of the App built with Express and MongoDB.

## Table of Contents

1. [User Authentication](#user-authentication)
2. [User Management](#user-management)
3. [Database Integration](#database-integration)
4. [API Endpoints](#api-endpoints)
5. [Client-side Features](#client-side-features)
6. [Middleware](#middleware)
7. [Environment Configuration](#environment-configuration)

## 1. User Authentication

- **Registration**: Users can create a new account by providing a username, email, and password.
- **Login**: Users can log in with their email and password to access the application.
- **JWT Authentication**: JSON Web Tokens (JWT) are used to secure API endpoints and manage user sessions.
- **Password Hashing**: User passwords are hashed using bcrypt before being stored in the database for added security.

## 2. User Management

- **Profile Management**: Users can view and update their profile information.
- **User Roles**: Different user roles (e.g., admin, user) can be assigned to control access to certain features.
- **Password Reset**: Users can reset their passwords if they forget them.

## 3. Database Integration

- **MongoDB**: The application uses MongoDB to store data.
- **Mongoose**: Mongoose is used to define schemas and interact with the MongoDB database.
- **Data Validation**: Mongoose schemas include data validation to ensure data integrity.

## 4. API Endpoints

### User Endpoints

- `POST /api/users/register`: Register a new user.
- `POST /api/users/login`: Authenticate a user and return a token.
- `GET /api/users/profile`: Get the authenticated user's profile.
- `PUT /api/users/profile`: Update the authenticated user's profile.

### Item Endpoints

- `GET /api/items`: Get a list of all items.
- `POST /api/items`: Create a new item.
- `GET /api/items/:id`: Get a single item by ID.
- `PUT /api/items/:id`: Update an item by ID.
- `DELETE /api/items/:id`: Delete an item by ID.

## 5. Client-side Features

- **React Integration**: The client side of the application is built with React.
- **Bootstrap**: Bootstrap is used for responsive design and UI components.
- **Axios**: Axios is used for making HTTP requests to the backend API.
- **Form Validation**: Client-side form validation is implemented for better user experience.

## 6. Middleware

- **Morgan**: HTTP request logger middleware for logging requests.
- **Body-Parser**: Middleware for parsing incoming request bodies.
- **Cookie-Parser**: Middleware for parsing cookies.
- **Error Handling**: Custom error handling middleware for catching and responding to errors.

## 7. Environment Configuration

- **dotenv**: Environment variables are managed using the `dotenv` package.
- **Configuration File**: Environment-specific configurations are stored in a `.env` file.

## Additional Features

- **EJS Templating**: EJS is used for server-side rendering of HTML templates.
- **Nodemon**: Nodemon is used during development to automatically restart the server on file changes.
- **Secure Passwords**: Passwords are stored securely using bcrypt hashing.

## Future Enhancements

- **Role-based Access Control**: Implement more granular access control based on user roles.
- **Pagination**: Add pagination for API endpoints that return lists of items.
- **Search and Filtering**: Implement search and filtering capabilities for items.
- **Testing**: Add unit and integration tests for critical parts of the application.

---

This document provides a high-level overview of the features available in the CRUD App. For more detailed information, refer to the project's source code and documentation.

### Additional Features

### Logged User Actions

Logged user can only perform the following actions:

- **Create Post**: Logged Users can create new blog posts.
- **Update Post**: Logged Users can only update existing blog posts.
- **Delete Post**: Logged Users can only delete their own blog posts.

These actions empower users to manage their content effectively and contribute to the blog community.

### File Upload

Users can upload files, such as images or documents, to include in their blog posts. The file upload feature enhances the multimedia capabilities of the blog app, allowing users to enrich their posts with visual or supplementary content.

Installation
Clone the repository:
https://github.com/Animace/Blog-FullStack




