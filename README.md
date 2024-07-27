# EasyBook Server
This repository contains the server-side code for EasyBook, a modern platform for book management and reading. Built with Express.js and MongoDB, this server provides a robust and secure backend to handle various functionalities, including user authentication, book management, and personalized recommendations.
### Features
● User Authentication: Secure login and registration using JSON Web Tokens (JWT). </br>
● Category Management: Create, read, update, and delete book categories.</br>
● Booking Management: Handle user bookings for books.</br>
● User Management: Manage user roles and permissions (admin, seller, buyer).</br>
● Advertisement Management: Feature and advertise selected books.</br>
● Secure Payment Processing: Integration with Stripe for payment handling.</br>
● Middleware: Utilizes CORS and JSON body parsing for smooth request handling</br>

### Technologies Used
● Node.js: JavaScript runtime for server-side development.</br>
● Express.js: Web framework for building RESTful APIs.</br>
● MongoDB: NoSQL database for scalable and flexible data storage.</br>
● JSON Web Token (JWT): Secure token-based authentication.</br>
 ●Stripe: Payment processing platform.</br>
● dotenv: For managing environment variables.</br>
● CORS: Middleware for enabling Cross-Origin Resource Sharing.</br>

## Endpoints
### Categories:
GET /category          - Retrieve all categories.</br>
GET /categories        - Retrieve all categories.</br>
POST /categories       - Create a new category.</br>
GET /categories/:name  - Retrieve categories by name.</br>
DELETE /categories/:id - Delete a category by ID.</br>
PATCH /categories/:id  - Update a category to be advertised.</br>

### Bookings:
GET /bookings          - Retrieve bookings by user email.</br>
POST /bookings         - Create a new booking.</br>

### Users:
GET /users             - Retrieve all users.</br>
POST /users            - Create a new user.</br>
POST /user             - Create a new user.</br>
GET /users/admin/:email- Check if a user is an admin.</br>
PUT /users/admin/:id   - Promote a user to admin (requires JWT).</br>
DELETE /users/:id      - Delete a user by ID (requires JWT).</br>
GET /users/seller      - Retrieve all sellers.</br>
GET /users/buyer       - Retrieve all buyers.</br>
GET /users/:email      - Retrieve a user by email.</br>

### Advertisements:
GET /advertised        - Retrieve all advertised books.</br>

### Advertisements:
GET /jwt               - Generate a JWT for a user.

## Dependencies
● express
● cors
● dotenv
● jsonwebtoken
● mongodb

# Live Link : <https://final-project-9df2d.web.app/>
