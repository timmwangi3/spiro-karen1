# Spiro Karen Web App

The main Spiro Karen product is a browser-based business system and PWA.

## End user
Open the web address in Chrome or Edge. No Windows installer is required.
On a supported HTTPS deployment, users can choose **Install Spiro Karen** from the browser to add it like an app.

## Includes
- POS and sales
- Tickets and QR verification
- Battery and station management
- Drivers and customers
- Swaps
- Payments / M-Pesa STK Push backend hooks
- Shifts and expenses
- Reports/dashboard
- PWA/offline shell
- Responsive PC/tablet/phone interface

## Run locally
Requirements: Node.js 20+.

```bash
npm install
npm start
```

Then open `http://localhost:8080`.

## PostgreSQL
Set `DATABASE_URL` and other production variables in `.env`. The supplied Docker Compose file provides PostgreSQL for development/deployment.

## Production
Use HTTPS, a strong `JWT_SECRET`, a real domain, backups, restricted database access, and real M-Pesa Daraja credentials/callback URL before taking payments.
