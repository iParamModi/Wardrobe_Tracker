# Wardrobe Tracker - MERN Stack Application

A full-stack web application to manage and organize wardrobe items using the MERN stack (MongoDB, Express.js, React, Node.js). Users can add cupboards, upload clothing details, manage washing status, and access the app through secure login.

## Features

- User and Admin authentication using JWT and cookies
- Add, update, delete cupboards
- Upload and manage clothing items with images
- Organize clothes by category
- Track washing and usage status
- File/image uploads with storage
- Protected routes using middleware
- CORS setup for frontend-backend communication

## Project Structure

backend/
  ├── controllers/
  ├── models/
  ├── routes/
  ├── middlewares/
  ├── db/
  ├── uploads/
  └── server.js
client/ (if frontend included)

## Tech Stack

- Frontend: React.js (if included)
- Backend: Node.js, Express.js
- Database: MongoDB (with Mongoose)
- Authentication: JWT, Cookies
- File Upload: multer (or manual)
- Middleware: for protected routes and token validation

## User Roles

- Admin: Manages users and has elevated permissions
- Client/User: Manages their wardrobe and clothes

## Installation and Setup

1. Clone the repository:
   git [clone](https://github.com/iParamModi/Wardrobe_Tracker.git) 
   cd wardrobe-tracker

2. Install backend dependencies:
   cd backend
   npm install

3. Create a `.env` file inside `backend/` and add the following:
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   FRONTEND_URL=http://localhost:3000

4. Start the backend server:
   node server.js

Backend will run on http://localhost:3002

## API Endpoints

POST   /cupboards/addCupboard         - Add a new cupboard  
GET    /cupboards/getCupboard         - Get all cupboards  
GET    /cupboards/getCupboardCount    - Get cupboard count  
PUT    /cupboards/updateCupboard      - Update cupboard info  
DELETE /cupboards/deleteCupboard/:id  - Delete a cupboard  
POST   /users/signup                  - Register admin user  
POST   /users/login                   - Login and get token  
POST   /users/logout                  - Logout and clear token  

## Author

Made by [Param Modi](https://github.com/iParamModi)

