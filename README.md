# Gasco Auto Service — Interactive Test Build

React/Vite prototype of the proposed public site, streamlined mechanic dashboard and customer portal.

## Local development
```bash
npm install
npm run dev
npm run build
```

## Important safety and functionality notes
- **Demo only.** This build intentionally uses localStorage for browser-local demo records. It has no secure shared backend, authentication, database, transactional email/SMS or payment processing. It is **not suitable for real customer personal information or production use**.
- Demo access buttons do not authenticate identities; real account login and role-based access must be implemented in a secure server-backed service before handling customers.
- Mechanic changes persist **in the same browser only**. They do not synchronize to another device or user.
- "Mark ready" changes the demo vehicle status. It does not dispatch a real text or email.
- Invoice entries are demo records, not legal invoices or payment requests.
- All customer data on first launch is synthetic. Do not enter real customer records in this preview.

## Production checklist
1. Secure authentication and role-based authorization with server-side row-level protections.
2. Shared database and migrations (customers, vehicles, work orders, checklist tasks, reminders, availability, appointments, invoices, messages).
3. Server-side booking conflict prevention and timezone-aware calendar.
4. Transactional notification provider and opt-in/opt-out and delivery logs.
5. Stripe/payment account integration and invoicing compliance.
6. Secure file storage, privacy policy, audit trail, backups, data deletion and QA across mechanic/customer accounts.
7. Verified domain, shop content and consent before public release.
