# Travelly — Install on Your Phone

Travelly is built as an installable **PWA** (Progressive Web App). It uses your phone's real
**GPS**, **live address search**, **maps**, **routing** and **weather** — and installs to your
home screen with its own icon, just like a native app.

The only requirement: a PWA must be opened from an **HTTPS link** (not a `file://` path) before the
phone will let you install it and use GPS. Pick **one** of the options below.

---

## Option A — Free hosting in ~2 minutes (recommended)

### Using Netlify Drop (no coding)
1. Go to **https://app.netlify.com/drop** on your computer.
2. Drag the whole **`app`** folder (this folder) onto the page.
3. Netlify gives you a live HTTPS link, e.g. `https://travelly-xyz.netlify.app`.
4. Open that link on your **phone's browser** (Chrome on Android, Safari on iOS).

### Or GitHub Pages
1. Create a free GitHub repo and upload the contents of this `app` folder.
2. Settings → Pages → Branch: `main`, folder: `/root` → Save.
3. Open the `https://<you>.github.io/<repo>/` link on your phone.

---

## Step 2 — Add it to your home screen

**Android (Chrome):**
- Tap the **⋮** menu → **Install app** / **Add to Home screen**.
- Or tap the black **"Install Travelly on your phone"** button that appears at the bottom.

**iPhone (Safari):**
- Tap the **Share** button (□↑) → **Add to Home Screen** → **Add**.

Travelly now has its own icon. Open it — it runs fullscreen with no browser bar.

---

## Step 3 — Allow location

The first time you open it, tap the **📍 button** (top-right of the map) and **Allow** location.
The map centres on you, shows a live blue dot, and address search results are biased to streets
near you.

---

## What works right now
- 🛰️ **Live GPS** current location + follow (blue dot, accuracy circle)
- 🔎 **Smart address autocomplete** — type a few letters of a street (e.g. "Warwick R") and pick the
  exact Rd / St / address from the dropdown
- 🗺️ **Real maps** (OpenStreetMap) + **real routing** (walk / cycle / drive) with live distance & time
- ⏱️ **Depart / Arrive** with date **and** time pickers
- 🌱 **Live trip tracking** — distance, kcal, CO₂ saved — plus trip history, insights, profile, help
- 🌤️ **Live weather** for your location

All map, search, routing and weather services used are **free and need no API key**
(OpenStreetMap, Photon, OSRM, Open-Meteo).

---

## Want a true native app instead? (Flutter APK)
The original prototype was Flutter. If your IFQ637 submission needs a native Android `.apk` /
iOS build, the next step is to scaffold the Flutter project from this same design. That needs the
Flutter SDK + Android Studio on your machine. Tell me and I'll generate the full Flutter codebase
to match this PWA screen-for-screen.
