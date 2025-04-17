# Career Quest - Backend

This is the backend for the **Career Quest** project. It provides user authentication features such as registration and login using Node.js, Express, and MongoDB.

## 📦 Tech Stack

- Node.js
- Express.js
- MongoDB (with Mongoose)
- bcryptjs (for password hashing)
- jsonwebtoken (optional, for future protected routes)
- CORS (to handle cross-origin requests)

---

## 🚀 Setup Instructions

### 1. Clone the Repository

bash
git clone https://github.com/poorvigoell/career-quest.git
cd career-quest/backend

2. Initialize Project & Install Dependencies
bash
Copy
Edit
npm init -y
npm install express mongoose bcryptjs jsonwebtoken cors

3. File Structure
pgsql
Copy
Edit
backend/
│
├── models/
│   └── User.js         # Mongoose user schema
│
├── routes/
│   └── auth.js         # Auth routes (register & login)
│
├── server.js           # Entry point
├── package.json

⚙️ How to Run
🧪 Development
bash
Copy
Edit
node server.js
OR (if using nodemon)

bash
Copy
Edit
npx nodemon server.js
Make sure MongoDB is running locally or update your connection string to MongoDB Atlas.

🛠️ API Endpoints
✅ Register User
POST /api/auth/register

Body:

json
Copy
Edit
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "yourpassword"
}
🔐 Login User
POST /api/auth/login

Body:

json
Copy
Edit
{
  "email": "john@example.com",
  "password": "yourpassword"
}
