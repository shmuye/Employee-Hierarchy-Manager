# Employee Hierarchy Manager

Application to manage employees and their reporting (manager) relationships.

The system allows users to:
- View employees
- Create employees
- Update employee information
- Delete employees
- Visualize and query the organization hierarchy

---

# Tech Stack

## Frontend
- Next.js 15
- React 19
- TypeScript
- Mantine UI
- Redux Toolkit
- React Query
- React Hook Form
- Zod
- Axios
- Tailwind CSS 4

## Backend
- Hono
- TypeScript
- PostgreSQL
- Drizzle ORM
- JWT Authentication
- Zod Validation

## Development Tools
- ESLint
- Vitest
- TSX
- Drizzle Kit

---

# Project Structure

```
├── frontend
│   ├── app
│   ├── components
│   ├── context
│   ├── lib
│   ├── types
│   ├── package.json
│   └── .env.example
│
├── backend
│   ├── drizzle
│   ├── src
│   │   ├── auth
│   │   ├── db
│   │   ├── middleware
│   │   ├── positions
│   │   ├── types
│   │   ├── users
│   │   ├── utils
│   │   ├── validations
│   │   └── index.ts
│   ├── test
│   ├── package.json
│   └── .env.example
│
└── README.md

```

---

# Environment Variables

## Backend (`backend/.env`)

Create a `.env` file inside the `backend` directory.

```env
DATABASE_URL=your_postgresql_connection_url
JWT_SECRET=your_secret_key
NODE_ENV=development
PORT=5000
```

## Frontend (`frontend/.env.local`)

Create a `.env.local` file inside the `frontend` directory.

```env
NEXT_PUBLIC_API_BASE_URL=http://localhost:5000
```

---

# Setup Instructions

## 1. Clone the Repository

```bash
git clone <your-repository-url>
cd Employee-Hierarchy-Manager
```

---

# Backend Setup

## 1. Navigate to Backend

```bash
cd backend
```

## 2. Install Dependencies

```bash
npm install
```

## 3. Configure Environment Variables

Create a `.env` file based on `.env.example`.

```bash
cp .env.example .env
```

Update the values accordingly.

## 4. Generate Database Schema

```bash
npm run db:generate
```

## 5. Run Database Migrations

```bash
npm run db:migrate
```

## 6. Start Development Server

```bash
npm run dev
```

Backend server will run on:

```bash
http://localhost:5000
```

---

# Frontend Setup

## 1. Navigate to Frontend

```bash
cd frontend
```

## 2. Install Dependencies

```bash
npm install
```

## 3. Configure Environment Variables

Create a `.env.local` file based on `.env.example`.

```bash
cp .env.example .env.local
```

Update the API URL if necessary.

## 4. Start Development Server

```bash
npm run dev
```

Frontend application will run on:

```bash
http://localhost:3000
```

---

# Available Scripts

## Frontend Scripts

```bash
npm run dev
```
Starts the Next.js development server.

```bash
npm run build
```
Builds the frontend for production.

```bash
npm run start
```
Starts the production server.

```bash
npm run lint
```
Runs ESLint.

---

## Backend Scripts

```bash
npm run dev
```
Starts the backend in watch mode.

```bash
npm run build
```
Compiles TypeScript files.

```bash
npm run start
```
Runs the production build.

```bash
npm run test
```
Runs tests using Vitest.

```bash
npm run db:generate
```
Generates Drizzle schema files.

```bash
npm run db:migrate
```
Runs database migrations.

```bash
npm run db:studio
```
Opens Drizzle Studio.

---

# Features

- Employee CRUD operations
- Manager and reporting hierarchy
- Organizational tree visualization
- REST API architecture
- JWT-based authentication
- Form validation using Zod
- State management with Context API
- API caching with React Query



