# Etec Api

## Description
This project is an API built with Express.js and MongoDB for managing an e-commerce system. It includes various middleware such as CORS, 
Helmet, Morgan, and Cookie Parser for security and performance optimizations. The API allows administrators to manage products, user authentication, 
and customer interactions efficiently.

## Features and Optimizations

### Performance Optimizations
- **Optimized Queries:** : Reducing unnecessary database queries to enhance response times.

### Main Features
- **Admin Dashboard:** Allows centralized management of products and orders.
- **User Authentication:** Secure login for users with session management.
- **CRUD Operations for Product Management:** Create, read, update, and delete products.
- **Limited Operations for Purchased Products:** Deleting and retrieving purchased products by users.
- **Limited Operations for Clients:** Deleting and retrieving client information.
- **Contact Management:** Tracking and managing client contacts.
- **Real-Time Updates:** Tracking products and order statuses in real-time.

### Security and Middleware
- **CORS:** Enables cross-origin requests for API access control.
- **Helmet:** Enhances security by setting various HTTP headers.
- **Morgan:** Logs HTTP requests for monitoring API usage.
- **Cookie Parser:** Parses cookies for session handling.

## Prerequisites
Before starting, make sure you have the following installed:
- [Node.js](https://nodejs.org/)
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) or local MongoDB installation

## Installation

### Back-End

1. Clone the project
   ```bash
   git clone https://github.com/Kodatchi-001/Etec-Api.git
   cd Etec-Api
   ```

2. Navigate to the back-end folder and install dependencies
   ```bash
   npm install
   ```

3. Configure your MongoDB connection in `backend/config/db.js` by replacing the connection details with your MongoDB URI.

4. Run the back-end server using `nodemon` (if you don't have `nodemon` installed, you can install it globally using `npm install -g nodemon`):
   ```bash
   npm start
   ```

5. The back-end server will be running at `http://localhost:5000`.

### Running the Full Stack

1. Ensure both the back-end and front-end servers are running on different ports:
   - **Back-End**: `http://localhost:5000`
   - **Front-End**: `http://localhost:3000`

2. Open your browser and navigate to `http://localhost:3000` to see the application in action.

## Main Dependencies

- *Express.js*: A framework to handle HTTP requests on the server side.
- *MongoDB*: NoSQL database to store the data.
- *Mongoose*: ODM to interact with MongoDB and simplify database operations.
- *CORS*: Middleware to handle cross-origin requests.
- *Helmet*: Middleware for securing HTTP headers.
- *Morgan*: HTTP request logger.
- *Cookie Parser*: Middleware for parsing cookies.

## Testing

### End-to-End (E2E) Testing
- The project includes end-to-end testing to ensure that the entire system works as expected from the user's perspective.

### Unit Testing
- Unit tests have been implemented to verify individual components and their functionalities.

The tests ensure that the API's functionality, security, and performance meet the required standards.
