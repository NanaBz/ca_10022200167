Nanakwaku Boateng Boakye-Akyeampong

Roll number: 10022200167

Cloud Application End‑of‑Semester Exam

Project: PANAYA E‑Commerce Web App

Overview
- Purpose: A modern e‑commerce site for PANAYA products, enabling shoppers to browse products, manage carts, place orders, and track payments/shipments.
- Stack: Next.js (App Router), React, TypeScript, Tailwind CSS, Prisma ORM, and a PostgreSQL‑ready schema.
- Structure: Admin and Shop portals with dedicated API routes under `src/app/api/*` and UI pages in `src/app/shop/*` and `src/app/admin/*`.

Live Demo
- Deployed URL: https://panaya-products.vercel.app

Core Features
- Product Catalog: List/detail views with images, categories, pricing, and stock.
- Shopping Cart: Client‑side cart with quantity adjustments, remove, totals, and shipping calculation.
- Authentication (basic flow): Redirect to login before protected actions like checkout.
- Orders & Order Items: Create orders from cart contents; persist line items and totals.
- Payments: Record payment attempts/status; designed to plug into a gateway.
- Shipments & Events: Create shipment records and event logs for simple tracking.
- Reviews: Capture user reviews/ratings linked to products and users.
- Admin Views: Manage products, categories, users, orders, payments, reviews, and shipments from the admin area.

Developer Notes
- API Endpoints: RESTful routes live under `src/app/api/*` (e.g., `/api/products`, `/api/orders`, `/api/payments`).
- Database Access: Centralized Prisma client in `src/lib/prisma.ts`; schema in `prisma/schema.prisma`.
- Utilities: Helpers for cart and general utilities in `src/lib/*`.

