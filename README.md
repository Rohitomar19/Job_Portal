🧑‍💼 Job Portal - MERN Stack Full-Stack Application
A robust and scalable Job Portal Web Application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) with modern tools like Clerk for authentication and Sentry for error tracking. The platform offers a role-based experience for Candidates and Recruiters with complete job management, application handling, secure login flows, and clean UI.

🚀 Tech Stack
Frontend:

React.js (with Vite for fast builds)

Tailwind CSS (utility-first responsive styling)

React Router

Clerk.dev (authentication & session management)

Axios for API communication

Backend:

Node.js

Express.js

MongoDB (with Mongoose)

Cloudinary (for resume & file uploads)

Sentry.io (error monitoring & logging)

dotenv for environment management

🧠 Key Concepts & What I Learned
Implementing role-based auth using Clerk (with protected routes and session state)

Creating secure backend APIs for job and user management

Uploading resumes via Cloudinary and storing file links

Frontend routing and protected navigation (React Router + Clerk)

Error tracking with Sentry for debugging production issues

Handling state & UI logic in a clean, modular React component structure

🔐 Authentication with Clerk.dev
This project uses Clerk to handle:

Secure signup/signin (passwordless + social providers)

Session tokens and route protection

Role-based redirection: Candidates and Recruiters have different dashboards

🛠 Features
✅ Candidate Side:
Register/Login with Clerk

Browse all available job listings

Apply to jobs with resume upload

Track applied jobs in personal dashboard

Edit personal profile & resume

✅ Recruiter Side:
Register/Login with Clerk

Post new job listings with description, salary, location, etc.

View all jobs posted by them

View list of candidates who applied

Delete job listings

📊 Common Features:
Role-based navigation & layout

Error feedback and toast notifications

Clean and responsive UI using Tailwind CSS

Error tracking using Sentry on both frontend & backend


📁 Folder Structure
📦 root
├── client (Frontend - React + Vite)
│   ├── public
│   ├── src
│   │     ├── assets
│   │     ├── components
│   │     ├── context
│   │     ├── pages
│   ├── index.html
│   ├── package.json
│   ├── tailwind.config.js
│   ├── postcss.config.cjs
│   ├── vite.config.js
│   ├── .gitignore
|   |──.env
│   └── README.md
│
├── server (Backend - Node + Express)
│   ├── config
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── uploads
│   ├── utils
│   ├── .env
│   ├── server.js
│   ├── package.json
│  
│
├── .gitignore


1. Setup backend

cd server
npm install
Create .env file with:
- MONGO_URI=
- CLOUDINARY_CLOUD_NAME=
- CLOUDINARY_API_KEY=
- CLOUDINARY_API_SECRET=
- SENTRY_DSN=
npm run dev

2. Setup frontend

cd ../client
npm install
VITE_CLERK_PUBLISHABLE_KEY=
VITE_API_URL=http://localhost:4000
npm run dev

🧪 Future Enhancements
Job filtering (by location, salary, keywords)

Email notifications on application

Admin panel for reporting and analytics

Pagination and infinite scroll

Dark mode toggle

🙌 Credits & Acknowledgements
Clerk.dev – Seamless authentication

Sentry.io – Production error monitoring

Cloudinary – File/media storage
