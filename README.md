# 📇 Contact Manager App

A simple **Contact Manager** built using **Node.js**, **Express.js**, and **MongoDB**.  
This project demonstrates how to build a RESTful API with authentication, error handling, and clean code structure.

---

## 🚀 Features
- Create, Read, Update, Delete (CRUD) contacts
- User authentication with **JWT**
- Password hashing with **bcrypt**
- Proper error handling with middleware
- Organized **MVC folder structure**
- MongoDB integration with **Mongoose**

---

## 🛠️ Tech Stack
- **Node.js**
- **Express.js**
- **MongoDB (Mongoose)**
- **JWT Authentication**
- **bcrypt**

---
## 📂 Project Structure
Contact-Manager-App/
│── controllers/ # Route logic
│── models/ # MongoDB schemas
│── routes/ # Express routes
│── middleware/ # Auth & error handler
│── config/ # Database connection
│── constants.js # Common status codes
│── server.js # App entry point

---

## ⚙️ Installation & Setup

**Clone the repository**
   git clone https://github.com/your-username/contact-manager-app.git
   cd contact-manager-app
   npm install
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   npm start


   
📌 API Endpoints
Authentication
Method	Endpoint	Description
POST	/api/users/register	Register new user
POST	/api/users/login	Login and get token
Contacts
Method	Endpoint	Description
GET	/api/contacts	Get all contacts
GET	/api/contacts/:id	Get single contact
POST	/api/contacts	Create new contact
PUT	/api/contacts/:id	Update contact
DELETE	/api/contacts/:id	Delete contact


🔒 Authentication
All contact routes are protected.
Use the token from /api/users/login in headers:
Authorization: Bearer <your_token>


📜 License
This project is licensed under the MIT License.
