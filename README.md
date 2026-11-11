# freshBite Pro v2 — Customer App + Admin Panel + API Starter

A clean, approachable food-ordering product starter for an Indian food business.

## Project structure
- `customer-app/` — Expo React Native Android/iOS customer app
- `admin-panel/` — responsive web admin dashboard (open `index.html` in a browser)
- `backend/` — Express REST API starter for products and orders

## 1) Run the customer app
Install Node.js, then:
```bash
cd customer-app
npm install
npx expo start
```
Install Expo Go on Android and scan the QR code.

## 2) Run the admin panel
Open `admin-panel/index.html` in Chrome/Edge. It currently demonstrates dashboard cards, sample orders, status updates, product listing and adding products in browser memory.

## 3) Run the API
```bash
cd backend
npm install
npm start
```
API starts at `http://localhost:4000`.
- `GET /health`
- `GET /api/products`
- `POST /api/products`
- `GET /api/orders`
- `POST /api/orders`
- `PATCH /api/orders/:id/status`

## Important: launch-readiness
This is a professional starter scaffold, not a finished production marketplace. Sample dashboard values and sample customer/order records are illustrative. The API stores data in memory and resets when restarted. It has no authentication, persistent database, delivery partner integration, live maps, notifications, or payment processing.

Before taking real orders:
1. Add PostgreSQL/MongoDB persistence and database migrations.
2. Add secure customer/admin authentication, password hashing, OTP verification, authorization and rate limiting.
3. Connect the customer app and admin panel to the API; use a deployed HTTPS API URL, not localhost on customer phones.
4. Integrate a regulated payment provider such as Razorpay using its official SDK and server-side order creation/signature verification/webhooks. Never store secret keys in the app or browser.
5. COD orders must be saved server-side; implement cancellation rules and order confirmation.
6. Add delivery address validation, serviceable pincode/radius, delivery fees, tax/GST invoices, refund/cancellation handling, inventory and customer support.
7. Replace remote demo photos with licensed images you have permission to use.
8. Add privacy policy, terms, refund policy, food/allergen information and business/legal compliance before public release.

## Growth basics
Start in one delivery zone, keep a focused menu, measure order conversion/repeat orders/cancellation/time-to-deliver, use honest offers, and expand only when operations are reliable.
