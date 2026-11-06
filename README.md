# ClearPath — Personal Budget

A lightweight, installable personal budgeting app built with plain HTML, CSS and JavaScript.

## Files

- `index.html` — the complete budgeting application
- `manifest.webmanifest` — installable web-app settings
- `sw.js` — service worker for offline app-shell caching

## Finance features

- Recurring bills with weekly, fortnightly, monthly, quarterly and yearly schedules; mark paid to create an expense and advance the next due date.
- Payday planner to allocate expected take-home pay across bills, essentials, savings, debt and discretionary spending.
- Debt tracker with balances, annual interest rates, minimum monthly repayments and estimated payoff/interest projections using a monthly amortisation estimate.
- `assets/logo.svg` — ClearPath logo
- `assets/favicon.svg` — browser tab icon
- `assets/icon-192.svg` and `assets/icon-512.svg` — app icons

## Deploy with GitHub Pages

1. Create a new **public** GitHub repository, for example `clearpath-budget`.
2. Extract this ZIP file on your computer.
3. Upload the **contents** of this folder to the repository's root. `index.html` must be visible at the top level, not inside another nested folder.
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch **main**, folder **/(root)**, then click **Save**.
7. Wait for GitHub Pages to publish. Your site URL will appear in the Pages section.

## Install on iPhone

1. Open the published HTTPS website in Safari.
2. Tap the Share icon.
3. Choose **Add to Home Screen**.
4. Confirm **Add**.

## Important data note

ClearPath stores its budget data in the browser's local storage on that device. It does not sync between devices and does not connect to bank accounts. Use the app's Export function to save regular JSON backups. Clearing browser/site data can remove locally stored transactions and goals.

## Updating the app

Replace the relevant files in the repository and commit the changes. If a previously installed app appears stale, close it fully and reopen it; if needed, clear the website data or update the service-worker cache version in `sw.js`.
