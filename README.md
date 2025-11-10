# Travel Package Website

This project is a simple travel package website with user authentication.

## Project Structure

```
│
├── backend/
│   ├── package.json
│   ├── server.js
│   ├── .env
│   ├── config/
│   │   └── db.js                # Database connection
│   ├── models/
│   │   └── User.js              # User schema/model
│   ├── routes/
│   │   └── authRoutes.js        # Signup/Login routes
│   ├── controllers/
│   │   └── authController.js    # Logic for signup/login
│   ├── middleware/
│   │   └── authMiddleware.js    # Verify JWT token
│   └── utils/
│       └── generateToken.js     # JWT generation helper
│
├── frontend/
│   ├── package.json
│   ├── vite.config.js
│   ├── src/
│   │   ├── main.jsx
│   │   ├── App.jsx
│   │   ├── components/
│   │   │   └── ProtectedRoute.jsx
│   │   ├── pages/
│   │   │   ├── Signup.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Home.jsx
│   │   ├── services/
│   │   │   └── api.js           # Axios instance
│   │   └── context/
│   │       └── AuthContext.jsx  # Manage auth state globally
│   └── public/
│       └── index.html
│
├── README.md                    # Project overview and setup guide
└── .gitignore
```

## Setup Guide

### Backend

1.  Navigate to the `backend` directory:
    ```bash
    cd backend
    ```
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Create a `.env` file and add your MongoDB connection string and a JWT secret:
    ```
    MONGO_URI=YOUR_MONGO_DB_URI
    JWT_SECRET=YOUR_JWT_SECRET
    ```
4.  Start the server:
    ```bash
    npm start
    ```

### Frontend

1.  Navigate to the `frontend` directory:
    ```bash
    cd frontend
    ```
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Start the development server:
    ```bash
    npm run dev
    ```
