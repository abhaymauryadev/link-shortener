# URL Shortener Backend

This is the backend for the URL Shortener application, built with Node.js, Express, and MongoDB.

## Features
- User registration and authentication (JWT-based)
- Create, manage, and track short URLs
- User dashboard for managing personal URLs
- RESTful API
- Error handling and middleware

## Project Structure
```
BACKEND/
  src/
    config/        # Configuration files (DB, app config)
    controller/    # Route controllers
    dao/           # Data access objects
    middleware/    # Express middlewares
    models/        # Mongoose models
    routes/        # API route definitions
    services/      # Business logic
    utils/         # Utility functions
  app.js           # Express app entry point
  package.json     # Project metadata and dependencies
```

## Setup
1. Install dependencies:
   ```bash
   npm install
   ```
2. Create a `.env` file in the BACKEND directory with the following variables:
   ```env
   PORT=5000
   MONGODB_URI=mongodb://localhost:27017/url_shortener
   JWT_SECRET=your_jwt_secret
   ```
3. Start the server:
   ```bash
   npm start
   ```

## Usage
- The backend runs on `http://localhost:5000` by default.
- Connect your frontend to this API (update base URL if needed).

## API Endpoints (Summary)
- `POST   /api/auth/register` — Register a new user
- `POST   /api/auth/login` — User login
- `GET    /api/user/profile` — Get user profile (auth required)
- `POST   /api/shorturl` — Create a short URL (auth required)
- `GET    /api/shorturl` — Get all URLs for user (auth required)
- `GET    /:shortId` — Redirect to original URL

