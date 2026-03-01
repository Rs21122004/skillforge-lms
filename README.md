# SkillForge — Learning Management System

A full-stack Learning Management System (LMS) built with **React**, **Node.js/Express**, and **MongoDB**. Features user authentication via **Clerk**, course browsing, course enrollment, and payment processing via **Stripe**.

## Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | React 19, Vite, Tailwind CSS 4, React Router |
| **Admin Panel** | React 19, Vite, Tailwind CSS 4 |
| **Backend** | Node.js, Express 5, Mongoose |
| **Database** | MongoDB Atlas |
| **Auth** | Clerk |
| **Payments** | Stripe |

## Project Structure

```
LMS/
├── frontend/      # Student-facing React app (port 5173)
├── admin/         # Admin panel React app (port 5174)
└── backend/       # Express API server (port 4000)
```

## Features

- 🔐 **Authentication** — Sign up, sign in, and protected routes via Clerk
- 📚 **Course Catalog** — Browse and search available courses
- 📖 **Course Details** — Detailed course pages with curriculum info
- 💳 **Payments** — Stripe-powered course enrollment
- 👨‍🏫 **Faculty Directory** — View instructors and their profiles
- 📋 **My Courses** — Track enrolled courses
- 🛠️ **Admin Panel** — Manage courses, view bookings, and dashboard analytics

## Getting Started

### Prerequisites

- **Node.js** v18+
- **npm** or **yarn**
- A [Clerk](https://clerk.com) account (for auth keys)
- A [Stripe](https://stripe.com) account (for payment keys)
- A [MongoDB Atlas](https://www.mongodb.com/atlas) cluster (or local MongoDB)

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/skillforge-lms.git
cd skillforge-lms
```

### 2. Set Up Environment Variables

Create `.env` files in each directory using the examples below:

**`backend/.env`**
```env
CLERK_SECRET_KEY=your_clerk_secret_key
CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
STRIPE_SECRET_KEY=your_stripe_secret_key
MONGO_URI=your_mongodb_connection_uri
```

**`frontend/.env`**
```env
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

**`admin/.env`**
```env
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

### 3. Install Dependencies

```bash
# Backend
cd backend && npm install

# Frontend
cd ../frontend && npm install

# Admin Panel
cd ../admin && npm install
```

### 4. Run the Application

Open three terminal windows:

```bash
# Terminal 1 — Backend (port 4000)
cd backend && npm start

# Terminal 2 — Frontend (port 5173)
cd frontend && npm run dev

# Terminal 3 — Admin Panel (port 5174)
cd admin && npm run dev
```

### 5. Open in Browser

- **Frontend:** [http://localhost:5173](http://localhost:5173)
- **Admin Panel:** [http://localhost:5174](http://localhost:5174)
- **API:** [http://localhost:4000](http://localhost:4000)

## Screenshots

> _Add screenshots of your running application here to make your portfolio stand out!_

## License

This project is for educational purposes.
