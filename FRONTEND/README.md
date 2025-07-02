# URL Shortener Frontend

This is the frontend for the URL Shortener application, built with React and Vite.

## Features
- User registration and login
- Create and manage short URLs
- Dashboard for user-specific URLs
- Responsive UI

## Project Structure
```
FRONTEND/
  src/
    api/           # API calls
    components/    # Reusable React components
    pages/         # Page components
    routing/       # Route definitions
    store/         # Redux store and slices
    utils/         # Utility functions
    index.css      # Global styles
    main.jsx       # App entry point
  index.html       # HTML template
  vite.config.js   # Vite configuration
```

## Setup
1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the development server:
   ```bash
   npm run dev
   ```

## Usage
- Visit the app in your browser at `http://localhost:5173` (default Vite port).
- Connects to the backend API (update API base URL in `src/utils/axiosInstance.js` if needed).


