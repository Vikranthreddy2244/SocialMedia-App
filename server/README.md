# Backend - SocioMedia

This is the backend of the SocioMedia application, built with Node.js, Express, and MongoDB.

## Features
- User authentication (register and login)
- CRUD operations for posts
- Friend management (add/remove friends)
- Middleware for token-based authentication
- File upload for user and post images

## Tech Stack
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Tokens (JWT)
- Multer (for file uploads)

## Setup Instructions

### Prerequisites
- Node.js installed
- MongoDB instance running
- `.env` file with the following variables:

```
PORT=8080
MONGO_URL=<your_mongo_connection_string>
JWT_SECRET=<your_jwt_secret>
```

### Installation
1. Navigate to the `server` directory:
   ```bash
   cd server
   ```
2. Install the dependencies:
   ```bash
   npm install
   ```
3. Start the server:
   ```bash
   npm start
   ```
4. The server will run on `http://localhost:8080`.

## API Endpoints

### Authentication
- **POST** `/auth/register` - Register a new user
- **POST** `/auth/login` - Login a user

### Users
- **GET** `/users/:id` - Get user details
- **GET** `/users/:id/friends` - Get user's friends
- **PATCH** `/users/:id/:friendId` - Add/remove a friend

### Posts
- **GET** `/posts` - Get all feed posts
- **GET** `/posts/:userId/posts` - Get posts by a specific user
- **POST** `/posts` - Create a new post
- **PATCH** `/posts/:id/like` - Like/unlike a post

## File Structure
- `routes/` - API routes
- `controllers/` - Business logic for routes
- `models/` - Mongoose schemas
- `middleware/` - Authentication middleware
- `data/` - Sample data for testing

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add feature-name"
   ```
4. Push to the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a pull request.