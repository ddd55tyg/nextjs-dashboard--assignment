# Demo Recording Script

Hi — this is a short script to follow while recording the dashboard demo.

1. Introduction (10-15s)
   - "Hi, I’m [Your Name]. This demo shows a responsive dashboard built with Next.js, Tailwind CSS, Redux Toolkit, and Recharts. I will demonstrate authentication, the data table, chart visualizations, exports, and Docker deployment."

2. Login (10-20s)
   - Show the /login page.
   - Use credentials: admin / password
   - Explain mocked API and where to replace with Firebase.

3. Data Table (45-60s)
   - Show sorting by different columns.
   - Use the search box to filter by name/email.
   - Change pages with pagination controls.
   - Click Export XLSX and Export PDF and show the downloaded files.

4. Chart (20-30s)
   - Show the Recharts line chart on the right.
   - Explain how chart reads from Redux state.

5. Docker (20-30s)
   - Show docker-compose.yml and explain how to run `docker-compose up --build`.
   - Mention port mapping (3000).

6. Wrap up (10s)
   - Mention next steps: replace mocked auth with Firebase, improve PDF layout with jspdf-autotable, and add server-side pagination for large datasets.

Tips:
- Use a screen recorder like OBS or Loom.
- Speak clearly and keep pauses short.
- Optional: show terminal commands when running the app or docker.
