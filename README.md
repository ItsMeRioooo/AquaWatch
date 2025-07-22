# AquaWatch - Real-Time Dam & River Water Level Dashboard

AquaWatch is a modern, real-time dashboard for monitoring dam and river water levels in the Philippines, powered by data from PAGASA. It features a beautiful, responsive UI and a robust backend scraper/caching system.

## Features

### 🌊 Real-Time Dashboard
- Displays the latest water level for any supported dam or river station.
- Shows last update timestamp and current alert/alarm level.
- Color-coded status indicator (Normal, 1st/2nd/3rd Alarm).
- Modern, responsive design with a clean, user-friendly interface.

### 📈 Interactive Chart
- Chart.js-powered line graph of the last 2 hours of readings (2h, 1h, 30m, Now).
- Visualizes water level trends for quick assessment.

### 📋 Details Table
- Tabbed interface: switch between Overview (chart) and Details (table).
- Details tab shows a table of recent readings, time periods, and change (delta) per interval.
- Color-coded change values (green for drop, red for rise).

### 🏞️ Multi-Station Support
- Dynamic dropdown to select from all available stations/dams.
- Station list is fetched from the backend and always up-to-date.

### 🔄 Auto-Refresh & Caching
- Data auto-refreshes every 10 minutes (configurable).
- Backend scrapes and caches data at fixed 10-minute intervals for reliability.
- Robust retry and fallback logic for scraping.

### 🛡️ Alarm Thresholds
- Per-station alarm thresholds (1st, 2nd, 3rd) shown in UI.
- Status and alarm colors update automatically based on latest reading.

### 🖥️ Debugging & Reliability
- Backend saves debug HTML and screenshots of the source site for troubleshooting.
- Logs scraping events and errors for easy monitoring.

### ⚡ Tech Stack
- Frontend: HTML, TailwindCSS, Chart.js, JavaScript
- Backend: Node.js, Express, Puppeteer

## Getting Started

1. `npm install` (install dependencies)
2. `node server.js` (start backend)
3. Open `index.html` in your browser (or serve via local web server)

## Data Source
- [PAGASA - Philippine Atmospheric, Geophysical and Astronomical Services Administration](https://pasig-marikina-tullahanffws.pagasa.dost.gov.ph/)

## License
MIT

---

© 2025 AquaWatch. All rights reserved.
