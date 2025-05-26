🛠️ Implementation Plan – Cadia
Phase 1: Local Development (Week 1–2)
Set up project structure on GitHub

Build core frontend in React (mobile-web hybrid)

Create REST API backend with Node.js on Ubuntu server

Use Docker to containerize app and ensure portability

Set up DNS routing to point to the Ubuntu server

Basic health check and monitoring with Uptime Kuma

Phase 2: MVP Features (Week 2–6)
Implement location-based solar time calculation

Add DST compensation logic

Integrate moon phase and sunrise/sunset APIs

Build UI for “Cadia Time,” current sleep suggestion, and wake alarm

Enable local notification logic for alarm and time events

Phase 3: Advanced Features (Week 6–10)
Integrate Schumann resonance data source (scrape or open API)

Solar activity integration (NOAA or similar)

Daily circadian report with visual elements

Sleep planning logic based on light phase + solar/lunar inputs

Store sleep logs in local DB with optional export

Phase 4: Stability + UX Polish (Week 10–12)
Mobile UI refinements and dark mode

Responsive PWA optimization

Test across devices and operating systems

Begin documentation for public deployment

Phase 5: Optional External Expansion
Add external authentication (OAuth or email-based)

Push to remote VPS or cloud if scale needed

Begin work on smartwatch support (Phase 6)