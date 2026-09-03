# ZELVORA — Secure Razorpay Setup

1. Create/activate your Razorpay merchant account.
2. Copy `.env.example` to `.env` on your server.
3. Add your Razorpay Key ID and Secret.
4. Run `npm install`, then `npm start`.
5. The backend creates Razorpay orders and verifies payment signatures.
6. Never expose the Razorpay secret key in frontend JavaScript.
7. Before production, use HTTPS, a database, server-side price/stock validation, authentication for admin routes, and Razorpay webhooks.
