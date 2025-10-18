# 📊 Dashboard Application (Next.js + Tailwind + Redux + Docker)

## 🎥 Recorded Demo Overview

This recorded demoshowcases a complete *Responsive Dashboard Application* built using *Next.js, React, Tailwind CSS, Redux Toolkit, and Recharts*.
URL:(https://drive.google.com/file/d/1CoCXny980GRMbtTH7B0yxwnVNuvlGg-u/view?usp=drivesdk)

The demo highlights:

- 🔐 *Authentication System* — Secure login and protected routes (with mocked API).
- 🖥️ *Responsive Dashboard* — Sidebar navigation, top bar with profile, and adaptive design for all screens.
- 📋 *Data Table Operations* — Sorting, filtering, pagination, and exporting data as *PDF* or *Excel*.
- 📈 *Chart Visualizations* — Dynamic charts using *Recharts*, updating automatically when data changes.
- 🐳 *Dockerized App* — Fully containerized and running in a lightweight Node.js environment.


## 🧠 Implementation Approach

### 1️⃣ Project Setup
- Initialized using create-next-app.
- Added *Tailwind CSS* for responsive UI design.
- Configured *PostCSS* and tailwind.config.js for custom utilities.

### 2️⃣ State Management
- Implemented *Redux Toolkit* for centralized state handling.
- Created dedicated slices for:
  - auth — managing login state.
  - data — handling table and chart data.

### 3️⃣ Authentication
- Built a *Login Page* using mocked API logic.
- Protected dashboard routes using conditional rendering based on auth state.

### 4️⃣ Dashboard Layout
- Created reusable UI components: Sidebar, Topbar, and MainContent.
- Used Tailwind utilities for grid and flex layouts.
- Fully responsive for desktop, tablet, and mobile.

### 5️⃣ Data Table Features
- Custom React table with:
  - 🔍 Filtering  
  - ↕️ Sorting  
  - ⏩ Pagination  
  - 💾 Export as PDF (via jsPDF) and Excel (via xlsx)
- Managed entirely through *Redux Toolkit* for real-time updates.

### 6️⃣ Chart Visualizations
- Built with *Recharts*.
- Displays summarized metrics dynamically linked to Redux state.
- Charts re-render instantly on data change.

### 7️⃣ Dockerization
Dockerfile:
```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build
EXPOSE 3000
CMD ["npm", "start"]
