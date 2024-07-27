# EasyBook Server
This repository contains the server-side code for EasyBook, a modern platform for book management and reading. Built with Express.js and MongoDB, this server provides a robust and secure backend to handle various functionalities, including user authentication, book management, and personalized recommendations.
### Features
● User Authentication: Secure login and registration using JSON Web Tokens (JWT).
● Category Management: Create, read, update, and delete book categories.
● Booking Management: Handle user bookings for books.
● User Management: Manage user roles and permissions (admin, seller, buyer).
● Advertisement Management: Feature and advertise selected books.
● Secure Payment Processing: Integration with Stripe for payment handling.
● Middleware: Utilizes CORS and JSON body parsing for smooth request handling

### Technologies Used
● Node.js: JavaScript runtime for server-side development.
● Express.js: Web framework for building RESTful APIs.
● MongoDB: NoSQL database for scalable and flexible data storage.
● JSON Web Token (JWT): Secure token-based authentication.
 ●Stripe: Payment processing platform.
● dotenv: For managing environment variables.
● CORS: Middleware for enabling Cross-Origin Resource Sharing.

## Endpoints
### Categories:
GET /category          - Retrieve all categories.
GET /categories        - Retrieve all categories.
POST /categories       - Create a new category.
GET /categories/:name  - Retrieve categories by name.
DELETE /categories/:id - Delete a category by ID.
PATCH /categories/:id  - Update a category to be advertised.

### Bookings:
GET /bookings          - Retrieve bookings by user email.
POST /bookings         - Create a new booking.

### Users:
GET /users             - Retrieve all users.
POST /users            - Create a new user.
POST /user             - Create a new user.
GET /users/admin/:email- Check if a user is an admin.
PUT /users/admin/:id   - Promote a user to admin (requires JWT).
DELETE /users/:id      - Delete a user by ID (requires JWT).
GET /users/seller      - Retrieve all sellers.
GET /users/buyer       - Retrieve all buyers.
GET /users/:email      - Retrieve a user by email.

### Advertisements:
GET /advertised        - Retrieve all advertised books.

### Advertisements:
GET /jwt               - Generate a JWT for a user.

## Dependencies
● express
● cors
● dotenv
● jsonwebtoken
● mongodb
