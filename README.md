# Traffly (Travelly) — Sustainable Journey Planner

A mobile travel app that helps you plan **sustainable routes**, tracks your trips live, and shows
your **CO₂ saved** and calories burned. Built for QUT **IFQ637**.

## Features
- 🛰️ **Live GPS** current location with follow-me (blue dot + accuracy circle)
- 🔎 **Smart address autocomplete** — type a few letters of a street and pick the exact Rd/St address
- 🗺️ **Real maps** (OpenStreetMap) and **routing** (OSRM) for walk / cycle / drive
- ⏱️ **Now / Depart / Arrive** journey timing with date **and** time pickers
- 🌱 **Live trip tracking** — distance, kcal, CO₂ saved
- 🧭 Trip history, multimodal trip timeline, saved routes
- 📊 Insights ("Your Impact") with monthly distance breakdown
- 🧑 Profile, Help Centre
- 📲 **Installable PWA** — add to your phone's home screen
- 🌤️ Live weather (Open-Meteo)

All location, map, routing and weather services are **free and need no API key**
(OpenStreetMap, Photon, OSRM, Open-Meteo).

## Project structure
```
Traffly/
├── app/                       # The installable mobile app (PWA)
│   ├── index.html             # Full application
│   ├── manifest.webmanifest   # PWA manifest
│   ├── sw.js                  # Service worker (offline + install)
│   ├── icon-192.png
│   ├── icon-512.png
│   └── HOW-TO-INSTALL.md      # Step-by-step phone install guide
├── travelly_prototype.html    # Early clickable prototype
└── README.md
```

## Run / install
See [`app/HOW-TO-INSTALL.md`](app/HOW-TO-INSTALL.md). In short: host the `app/` folder on any
free HTTPS host (e.g. Netlify Drop), open the link on your phone, then **Add to Home Screen**.

To run locally on a computer:
```bash
cd app
python3 -m http.server 8000
# open http://localhost:8000
```
(GPS works on `localhost` and over HTTPS only.)

## Roadmap
- Native Flutter build (Android APK / iOS) matching this design
- Real public-transport routes (bus / ferry timetables)
- Persistent trip history & real login/profile
