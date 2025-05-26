🧰 Tech Stack for Ubuntu Server (Markdown)
Frontend
React – UI framework for building the app

Vite – fast local dev server and build tool

TypeScript – strongly typed frontend logic

Tailwind CSS – rapid utility-first styling

PWA – service workers to make the app installable and offline-friendly

Backend
Node.js + Express – REST API to serve time, resonance, and sleep data

MongoDB – local database for sleep logs and user settings (can be swapped for PostgreSQL if preferred)

Docker – containerize backend and frontend for modular deployment

PM2 – keep Node.js backend process alive

Nginx – reverse proxy for serving frontend and routing API calls

Hosting & DevOps
Ubuntu Server – self-hosted environment

DNS Routing – configured via your domain registrar to point to your home IP (use Dynamic DNS if IP is not static)

UFW – firewall management

Let's Encrypt + Certbot – free HTTPS/SSL support

Fail2Ban – basic server protection

APIs & Data Sources
Sunrise/Sunset API – https://sunrise-sunset.org/api

Moon Phase API – https://api.farmsense.net/v1/moonphases/

DST & Timezone API – https://worldtimeapi.org/

Schumann Resonance – scraped from public sources like HeartMath

Solar Activity (NOAA) – https://services.swpc.noaa.gov/json/

Monitoring & Logs
Uptime Kuma – self-hosted uptime monitor (runs on Docker)

Logrotate – manage log file sizes on server

Netdata – system metrics monitoring