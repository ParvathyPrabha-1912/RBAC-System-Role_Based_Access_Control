# RBAC-System-Role_Based_Access_Control--System
The project contains entire code for login page for admin,sign up page for users.The New project is created by admin and the designer,developer and tester being selected by an admin. Workflow will be maintained based on their role.Google firebase is used for the backend process which best suits the quick response.

Features
  Manage roles and their permissions.
  Assign roles to users and control their access.
  RESTful API support for seamless integration.
  Secure and scalable design.

Project Structure

  Role-Based-Access-Control-RBAC-System/  
  │  
  ├── controllers/          # Controllers to handle requests and business logic  
  ├── models/               # Database models and schema definitions  
  ├── routes/               # API route definitions  
  ├── middleware/           # Middleware for authentication and authorization  
  ├── config/               # Configuration files for database and environment  
  ├── utils/                # Utility functions and helpers  
  ├── tests/                # Test cases for features  
  ├── package.json          # Node.js dependencies and scripts  
  ├── README.md             # Project documentation  
  └── .env                  # Environment variables  
  
Installation

1.Clone the repositary-- git clone https://github.com/ParvathyPrabha-1912/RBAC-System-Role_Based_Access_Control.git
2.Navigate to the project directory--cd RBAC-System-Role_Based_Access_Control--System
3.Install dependencies--npm install
4.Run the application--npm start




API Endpoints


Roles
POST /roles - Create a new role.
GET /roles - Fetch all roles.
PATCH /roles/:id - Update a role.
DELETE /roles/:id - Delete a role.


Users
POST /users - Create a new user.
GET /users - Fetch all users.
PATCH /users/:id - Update user details.
DELETE /users/:id - Delete a user.


Authentication
POST /auth/login - Log in a user and generate a JWT.
POST /auth/register - Register a new user.

Usage

1.Assign roles to users during registration or using the API.
2.Secure your endpoints by adding RBAC middleware to verify permissions:

const authorize = require('./middleware/authorize');  
app.use('/secure-endpoint', authorize('role_name'));  

Testing--npm test


  
