# Next.js Tailwind Redux Dashboard

This project is a starter dashboard built with Next.js, Tailwind CSS, Redux Toolkit and Recharts.

## What's included
- Mocked authentication API (`/pages/api/auth.js`) with credentials: `admin` / `password`
- Login page (`/pages/login.js`) that calls the API
- Data table (sorting, filtering, pagination) with XLSX and PDF export
- Chart (Recharts)
- Redux Toolkit store
- Tailwind CSS setup
- Dockerfile & docker-compose

## How to run locally

1. Install dependencies:
   ```bash
   npm install
   ```
2. Run dev server:
   ```bash
   npm run dev
   ```
3. Open http://localhost:3000

## Mock credentials
- username: `admin`
- password: `password`

## Docker
```bash
docker-compose up --build
```

## Demo recording script (included in repo as `DEMO_SCRIPT.md`)
Follow the script to record a screen demo explaining the project.

## To include your recorded demo
Replace the file `demo-recording-placeholder.txt` with your recorded video (e.g. `demo.mp4`) in the repo root, then push to GitHub or keep it alongside the ZIP.

## Notes
- For production replace mocked auth with Firebase or a real backend.
- PDF export is basic; for production consider `jspdf-autotable`.
