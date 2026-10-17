# RL-INSTITUTE Student Management Portal

A responsive, premium-style front-end prototype for a small tutoring institute. Built as a self-contained HTML file so it can be hosted as a static site (for example, with GitHub Pages).

## What's included
- Student directory: add, edit, search, delete
- Daily attendance register
- Fee payments, balances and transaction history
- Test marks and grades
- Branded printable report cards (browser Print / Save as PDF)
- WhatsApp fee-reminder composer (opens a prefilled WhatsApp chat; the user still taps Send)
- CSV exports and JSON backup/restore
- Fictional demo records
- Responsive layout for desktop and Android mobile

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a modern browser.
3. Choose **Settings & Backup → Load / reset demo data** to explore.
4. Data is saved in the browser's local storage.

## Upload to GitHub Pages
1. Create a new GitHub repository, e.g. `rl-institute-portal`.
2. Upload `index.html`, `README.md`, and `SUPABASE_STARTER.sql`.
3. In the repository, open **Settings → Pages**.
4. Choose deployment from the `main` branch and `/ (root)`, then save.
5. GitHub will show the public site URL after deployment.

## Important production limitation
This version is a front-end prototype. Browser local storage is device/browser-specific, has no secure login, is not shared across devices, and is not a secure database. Do not use it for real student personal records on a public website yet.

For a production version, connect Supabase (database + authentication), enable Row Level Security (RLS) for every table, restrict data to authorised institute users, and test the policies before adding actual student data. `SUPABASE_STARTER.sql` is only a starting schema and must be reviewed and secured; it does not automatically connect this HTML app to Supabase.

## WhatsApp reminders
Phone number must include country code with digits only (for example, India: `91` followed by the mobile number). The app opens WhatsApp with a pre-filled message; the operator must review and press Send. It does not send messages automatically.

## Privacy
Use fictional data while testing. Never upload real student names, parent phone numbers, fee information, or marks to a public GitHub repository.
