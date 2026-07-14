# IMDB Clone Technical Assessment

## Bug Report

## Bug Report

Google Doc: <https://docs.google.com/document/d/14SnAvWoupzz7DjHZY40Uh-JCzN2GUl9B41CtN2hc2jY/edit?usp=sharing>

---

# Project Setup

## Prerequisites

- Node.js 22.x
- npm

## Installation

Clone the repository

```bash
git clone https://github.com/akash200424/IMDB-Debug-Assesment.git
cd IMDB-Debug-Assesment
```

Install backend dependencies

```bash
npm install
```

Install frontend dependencies

```bash
cd client
npm install
cd ..
```

---

# Environment Configuration

Create a `.env` file in the project root.

Example:

```env
PORT=5000
JWT_SECRET=your_super_secret_jwt_key_here
```

---

# Database Setup

Run migrations

```bash
npx knex migrate:latest
```

Seed the database

```bash
npm run seed
```

---

# Run the application

```bash
npm run dev
```

Backend

```
http://localhost:5000
```

Frontend

```
http://localhost:5173
```

(Vite may automatically choose another available port if 5173 is already in use.)

---

# Assumptions

- SQLite is used as the local development database.
- Environment variables are provided through a `.env` file.
- Seed data is loaded using Knex.

---

# Bugs Fixed

- Fixed the incorrect database seed script to use Knex seed execution.
- Added the missing project dependencies required to run the application.
- Corrected the backend CORS origin configuration.
- Fixed login error handling so authentication failures display appropriate feedback.
- Optimized the Producer page by preventing unnecessary API requests caused by an incorrect React `useEffect` implementation.

---

# Additional Notes

- Database migrations and seed files are included.
- Bug report is available in the linked Google Document.
- All fixes were committed incrementally to demonstrate the debugging process.
