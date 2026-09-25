# Payment & Employee Dashboard

A single-page HR dashboard (pure HTML/CSS/JS, no build step) with two tabs:

- **Payment Disbursement** – track payment name, total amount, total payment, balance, sent/payment dates, delay days and status.
- **Employee Details** – track employee code, name, designation, branch, net payable, month, status and remarks.

## Features
- Add / edit / delete records via modal forms
- Bulk select & delete
- Filter by status, name/branch/designation, month, and date range
- Import data from CSV
- Export data to CSV
- Data persisted in the browser via `localStorage`
- Light/dark theme aware (follows system preference)

## Usage
Just open `index.html` in any modern browser — no server or dependencies required.

### Run locally
```bash
git clone <this-repo-url>
cd <repo-folder>
open index.html   # or double-click the file
```

### Deploy with GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under "Build and deployment", select **Deploy from a branch**, choose the `main` branch and `/ (root)` folder.
4. Your dashboard will be live at `https://<username>.github.io/<repo-name>/`.

## Notes
- All data is stored locally in the browser (`localStorage`), so it is per-device/per-browser and not shared between users.
- CSV import/export uses simple comma splitting — avoid commas inside field values when preparing import files.
