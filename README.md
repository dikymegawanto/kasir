# Next.js Kasir (Pages Router) - Simple POS + Self-order

This is a simple cashier application built with Next.js (Pages Router) and PostgreSQL using Prisma.
Features:
- Menu with ingredients; menu disabled when any ingredient stock insufficient.
- CRUD for menus & ingredients.
- POS for cashier (add to cart, checkout, print receipt).
- Self-order for customers (orders go to cashier).
- PostgreSQL via Prisma (schema + seed included).

## Quick start
1. Copy `.env.example` to `.env` and update `DATABASE_URL`.
2. Install deps: `npm install`
3. Generate Prisma client: `npx prisma generate`
4. Run migration: `npx prisma migrate dev --name init`
5. Seed data: `node prisma/seed.js`
6. Start dev server: `npm run dev`

Open http://localhost:3000 (POS), /self-order (customer), /admin (CRUD).
