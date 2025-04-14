# Node Task Manager

A simple task management API built with Node.js, Express, and MongoDB. It supports user authentication using JWT and provides endpoints for creating, retrieving, updating, and deleting tasks.

## Features

- User registration and authentication
- JWT-based session management
- CRUD operations for tasks
- MongoDB integration via Mongoose
- Environment-based configuration
- Jest testing framework integration

## Live Demo

The API is hosted on **Render** and available at:

👉 [https://task-manager-app-demo-sa.onrender.com/](https://task-manager-app-demo-sa.onrender.com/)

You can use tools like Postman or cURL to interact with the API.

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v14 or later)
- [MongoDB](https://www.mongodb.com/) instance (local or cloud)

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/siddhant197/node-task-manager.git
   cd node-task-manager
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Configure environment variables:

   - Create a `.env` file in the root directory.
   - Define the following variables:

     ```env
     JWT_SECRET=your_jwt_secret
     MONGODB_URL=your_mongodb_connection_string
     ```

   - For testing purposes, create a `.env.test` file with appropriate test configurations.

4. Start the development server:

   ```bash
   npm run dev
   ```

   The server will start on `http://localhost:3000`.

## Running Tests

The project uses Jest for testing. To run the test suite:

```bash
npm test
```

Ensure that your `.env.test` file is properly configured before running tests.

## API Endpoints

- `POST /users`: Register a new user
- `POST /users/login`: Authenticate a user
- `POST /tasks`: Create a new task
- `GET /tasks`: Retrieve all tasks
- `GET /tasks/:id`: Retrieve a specific task
- `PATCH /tasks/:id`: Update a task
- `DELETE /tasks/:id`: Delete a task

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License.
