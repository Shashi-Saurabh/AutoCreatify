# 🚀 AutoCreatify

AutoCreatify is a full-stack application that empowers users to generate, publish, and engage with AI‑driven creations — including images and text. Built with a modern MERN-like stack (React + Node + PostgreSQL), it includes features like user authentication, content creation, publishing, and community interactions like liking others' content.

---

## 🔗 Live Demo

- **Frontend (Client)**: [https://auto-creatify.vercel.app](https://auto-creatify.vercel.app)
- **Backend (API)**: [https://auto-creatify-server.vercel.app](https://auto-creatify-server.vercel.app)

---

## ✨ Features

- 🔐 **Authentication** via Clerk
- 🖼️ **AI Image & Markdown Creation**
- 📤 **Publish** content to the community
- 🧑‍💻 **User Dashboard** to manage your creations
- ❤️ **Like / Unlike** functionality with real-time updates
- 🌐 **Responsive Design** with Tailwind CSS

---

## 🧰 Tech Stack

| Layer        | Tech Used                              |
| ------------ | -------------------------------------- |
| Frontend     | React, Tailwind CSS, react-markdown    |
| Backend      | Node.js, Express.js                    |
| Auth         | Clerk                                  |
| Database     | PostgreSQL (with `postgres` library)   |
| Deployment   | Vercel (client + server)               |

---

## 📁 Project Structure

AutoCreatify/
├── client/ # React frontend
│ ├── src/
│ │ ├── components/ # UI Components
│ │ ├── assets/ # Static images/data
│ │ └── pages/ # App pages
│ ├── public/
│ └── package.json
├── server/ # Express backend
│ ├── configs/ # DB config
│ ├── controllers/ # Route logic
│ ├── routers/ # Route endpoints
│ ├── middlewares/ # Auth and error middlewares
│ └── package.json
├── README.md
└── .gitignore

yaml
Copy code

---

## ⚙️ Getting Started

### 🛠️ Prerequisites

- Node.js v18+
- PostgreSQL database
- Clerk account (for auth)
- Vercel account (for deployment)

---

### 🔧 Backend Setup

```bash
cd server
npm install
Create a .env file in server/:

env
Copy code
DATABASE_URL=postgres://user:password@host:port/database
CLERK_API_KEY=your_clerk_api_key
CLERK_JWT_KEY=your_clerk_jwt_key
PORT=4000
Run the backend server:

bash
Copy code
npm run dev
💻 Frontend Setup
bash
Copy code
cd client
npm install
Create a .env file in client/:

env
Copy code
VITE_BASE_URL=https://auto-creatify-server.vercel.app
Run the frontend:

bash
Copy code
npm run dev
Visit: http://localhost:5173

📦 API Endpoints
Method	Endpoint	Description
GET	/api/user/get-user-creations	Fetch user’s own creations
GET	/api/user/get-published-creations	Get all published community creations
POST	/api/user/toggle-like-creation	Like/Unlike a creation


🤝 Contributing
Contributions, issues, and feature requests are welcome!

Fork the repo

Create a new branch (git checkout -b feature-name)

Make your changes

Commit (git commit -m 'Add feature')

Push (git push origin feature-name)

Open a Pull Request

👨‍💻 Author
Shashi Saurabh
GitHub: @Shashi-Saurabh
