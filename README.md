# Blog App Features

This blog app comes with several features implemented on both the server-side and the client-side.

#Full Authentication
User Registration: Users can register with their name, email, and password.
User Login: Secure login using JWTs and HTTP-only cookies.
User Roles: Assign roles (admin, user) to manage access control.

#Technology Stack
Frontend: React, React-Bootstrap, React-Router, Redux Toolkit
Backend: Node.js, Express.js
Database: MongoDB
Authentication: JWT

### Additional Features

### Logged User Actions

Logged user can only perform the following actions:

- **Create Post**: Logged Users can create new blog posts.
- **Update Post**: Logged Users can only update existing blog posts.
- **Delete Post**: Logged Users can only delete their own blog posts.

These actions empower users to manage their content effectively and contribute to the blog community.

### File Upload

Users can upload files, such as images or documents, to include in their blog posts. The file upload feature enhances the multimedia capabilities of the blog app, allowing users to enrich their posts with visual or supplementary content.




