# 🔐 MERN Stack - User Authentication & Authorization

This is a full-stack MERN application that demonstrates **User Authentication and Authorization** using **MongoDB, Express.js, React.js, and Node.js**. Users can register, login, and access protected routes based on their roles (User/Admin).

## 📚 Tech Stack

- **Frontend**: React.js, Axios, React Router
- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT (JSON Web Tokens), bcrypt
- **Authorization**: Role-based access control

## ✅ Features

- ✅ User Registration with hashed passwords
- ✅ User Login with JWT token
- ✅ Protected Routes
- ✅ Role-based Authorization (Admin/User)
- ✅ Token saved in localStorage
- ✅ Logout functionality
- ✅ Clean code structure with error handling

## 📂 Project Folder Structure

```
mern-auth/
├── backend/
│   ├── config/           → DB and environment config
│   ├── controllers/      → Business logic
│   ├── middlewares/      → JWT & role protection
│   ├── models/           → Mongoose models
│   ├── routes/           → API endpoints
│   └── server.js         → Entry point
├── frontend/
│   ├── src/
│   │   ├── components/   → Reusable UI
│   │   ├── pages/        → Login, Register, Dashboard, etc.
│   │   ├── App.js
│   │   └── index.js
│   └── public/
├── .env
└── README.md
```

## 🛠️ Getting Started

### 🧩 Prerequisites

- Node.js installed
- MongoDB running locally or a MongoDB Atlas URI

### 📦 Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside `/backend` and add the following:

```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
```

Start backend server:

```bash
npm start
```

### 🖥️ Frontend Setup

```bash
cd frontend
npm install
npm start
```

Runs on: `http://localhost:3000`

## 🔐 API Endpoints

| Method | Route              | Description            | Access     |
|--------|--------------------|------------------------|------------|
| POST   | /api/auth/register | Register new user      | Public     |
| POST   | /api/auth/login    | Login & get JWT token  | Public     |
| GET    | /api/user/profile  | User profile details   | Protected  |
| GET    | /api/admin/users   | List of all users      | Admin Only |

## 🛡️ Role-Based Access

- **User**: Can register, login, access profile.
- **Admin**: Can access admin-only routes.
- Protected using JWT authentication and middleware.

## 📸 Screenshots

_Add your app screenshots here to showcase UI and functionality_

## 💡 Future Improvements

- Email verification
- Password reset via email
- Social login (Google/Facebook)
- Dark mode for UI

## 🙋‍♂️ Author

**Gaurav Yadav**  
GitHub: [https://github.com/gaurav-opensource](https://github.com/gaurav-opensource)
