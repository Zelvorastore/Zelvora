# ZELVORA Admin & Orders

This version adds a SQLite database and protected admin APIs.

## Start
1. Copy `.env.example` to `.env`.
2. Set `ADMIN_TOKEN` to a long random secret.
3. Add Razorpay keys when you are ready for online payments.
4. Run `npm install`.
5. Run `npm start`.

## API
GET `/api/products` — active storefront products.
POST `/api/orders` — create an order.
GET `/api/admin/orders` — admin order list (Bearer ADMIN_TOKEN).
GET `/api/admin/products` — admin product list.
POST `/api/admin/products` — add product (admin token).
PATCH `/api/admin/orders/:id` — update order/payment status (admin token).

For production, deploy behind HTTPS, use strong admin authentication/roles, server-side cart/product validation, backups, monitoring and payment webhooks.
