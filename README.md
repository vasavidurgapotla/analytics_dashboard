📊 MERN Analytics Dashboard 

A production-oriented, full-stack analytics dashboard built with the MERN stack, designed to mirror real-world SaaS and internal admin platforms used by distributed teams.

The application focuses on data aggregation, visualization, predictable state management, and secure access control, demonstrating the skills required for remote MERN / full-stack roles.

🌍 Live Demo
👉 https://dashboard-mern-tau.vercel.app/

This project showcases my ability to:

Build scalable dashboards used by businesses and SaaS products

Design clean frontend architectures for long-term maintainability

Implement secure authentication & role-based access

Manage global application state using Redux Toolkit

Work with API-driven data visualization

Deploy and maintain full-stack applications remotely

It reflects the type of work commonly done in remote-first teams, including async development, API contracts, and separation of concerns.

🧩 Core Features

📈 Interactive analytics charts (Line, Bar, Pie) using Recharts

🗂️ Predictable global state management with Redux Toolkit

📊 API-driven dashboards with aggregated backend data

🧾 Tabular data views with status indicators

🔐 JWT-based authentication

🛡️ Role-based authorization (admin / user)

🔒 Protected frontend & backend routes

⚡ Responsive admin-style UI suitable for desktop & tablet

🧱 Modular, scalable codebase

🧠 Architecture Overview
Frontend

Built with React using a feature-based structure

Redux Toolkit manages shared state (analytics data, user session, dashboard metrics)

Recharts renders visual analytics from API responses

ProtectedRoute ensures only authorized users access sensitive views

API layer abstracts backend communication

Backend

RESTful API built with Express.js

Controller–Route–Model pattern for clarity and scalability

MongoDB with Mongoose for structured data modeling

JWT authentication with role & admin middleware

Designed for easy extension (new metrics, reports, roles)

🛠️ Tech Stack
Frontend

React

Redux Toolkit

Recharts

Axios

Tailwind CSS

Backend

Node.js

Express.js

MongoDB

Mongoose

JWT Authentication

Deployment

Frontend: Vercel

Backend: Railway

Database: MongoDB Atlas

📁 Project Structure
├── client        # React frontend
├── server        # Node.js backend
└── README.md

📁 Frontend Structure (Scalable & Team-Friendly)
client/
└── src/
    ├── api/                  # API services & requests
    ├── components/           # Reusable UI components
    │   ├── charts/           # Analytics charts
    │   ├── tables/           # Data tables
    │   ├── layout/           # Sidebar, Navbar, Layouts
    │   └── ui/               # Shared UI elements
    ├── pages/                # Feature-based pages
    ├── redux/                # Store & slices
    ├── routes/               # Routing & access control
    ├── hooks/                # Custom hooks
    ├── utils/                # Helpers
    └── styles/               # Global styles

Redux Design Decisions

Redux Toolkit chosen for predictable state updates

Centralized analytics data avoids prop drilling

Enables consistent UI updates across charts and tables

Easy to extend with new slices and async thunks

📁 Backend Structure (Production-Ready)
server/
├── controllers/     # Business logic
├── routes/          # API endpoints
├── models/          # Mongoose schemas
├── middlewares/     # Auth & role control
├── config/          # DB & JWT utilities
└── server.js        # App entry point

Security

JWT-based authentication

Role & admin authorization middleware

Protected routes for sensitive operations

⚙️ Local Setup
Prerequisites

Node.js (v16+)

MongoDB (local or Atlas)

Installation
git clone https://github.com/your-username/analytics-dashboard.git
cd analytics-dashboard

Backend
cd server
npm install
npm run dev

Frontend
cd client
npm install
npm start

🔑 Environment Variables

Create a .env file inside server/:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key

Includes:

Dashboard overview

Analytics charts

User & company management

Admin views
(See screenshots above)

🚀 Future Improvements (Planned)

🌙 Dark mode

📅 Advanced filters & date ranges

📤 CSV / PDF export

🔄 Real-time updates (WebSockets)

🔐 Fine-grained role permissions

🧪 Automated tests

📄 License

