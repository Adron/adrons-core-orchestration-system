# Adron's Core Orchestration System

A modern web application built with Next.js, React, PostgreSQL, and Prisma.

## Development Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the development database:
   ```bash
   docker-compose up -d
   ```

3. Run Prisma migrations:
   ```bash
   npx prisma migrate dev
   ```

4. Start the development server:
   ```bash
   npm run dev
   ```

The application will be available at `http://localhost:3000`

## Production Deployment (Vercel)

1. Push your code to a Git repository

2. Create a new project on Vercel and connect it to your repository

3. Set the following environment variables in Vercel:
   - `DATABASE_URL`: Your production PostgreSQL connection string
   - `NODE_ENV`: "production"

4. Deploy the application

## Database Management

- Generate Prisma Client:
  ```bash
  npx prisma generate
  ```

- Create a migration:
  ```bash
  npx prisma migrate dev
  ```

- Reset the database:
  ```bash
  npx prisma migrate reset
  ```

## Tech Stack

- Next.js (App Router)
- React
- PostgreSQL
- Prisma
- TypeScript
- Tailwind CSS
- ESLint
