# Stockly - work completed as of 12 Oct 2026

Matches the Gantt chart (5 Oct - 4 Nov 2026).

## Week 1 - DONE: Authentication & role management
- app/api/auth/* (register, login, logout, session, Google OAuth)
- app/login, app/register, contexts/auth-context.tsx
- utils/auth.ts, utils/auth.client.ts (JWT cookie sessions, bcrypt)
- proxy.ts + middleware/authMiddleware.ts (route protection, role checks)
- lib/validations/auth.ts, lib/env.ts

## Week 1-2 - IN PROGRESS: Backend API structure & database models
- prisma/schema.prisma (MongoDB models), prisma/client.ts, prisma/*.ts data helpers
- app/api/products, categories, suppliers, health (REST route handlers)
- lib/api/* (client, errors, response helpers, rate limit)

## Not started yet (not included)
Stock data API integration, watchlist backend, portfolio/transactions,
API validation & error handling pass.

## Run
cp .env.example .env   # set DATABASE_URL, JWT_SECRET, NEXT_PUBLIC_API_URL
npm install && npm run dev
