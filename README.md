[README.md](https://github.com/user-attachments/files/33960227/README.md)
# 🛡️ KSHETRA — Tactical Airspace Intelligence & Counter-Drone Defense System

> **Next-Generation Autonomous Airspace Surveillance, Kinetic Deconfliction & 3D Threat Telemetry C2 Platform**

---

## 📌 Overview

**KSHETRA** (क्षेत्र) is a mission-critical, enterprise-grade Tactical Command and Control (C2) situational awareness simulation console. Built with real-time vector kinematics, Three.js 3D volumetric models, multi-sector radar fusion, and Supabase Realtime multi-operator synchronization, KSHETRA enables defense operators to track, classify, and mitigate aerial intrusions in high-stakes operational sectors.

---

## 🚀 Key Features

### 1. Dual Command Consoles
- **Standard C2 Console (`/`):** React + Framer Motion high-performance cockpit interface featuring interactive tactical maps, real-time telemetry tables, event dossiers, sector filtering, and operator callsign synchronization.
- **Advanced Tactical View (`/advanced-console.html`):** Deep-space 3D tactical radar suite featuring RF jamming cones, dynamic no-fly zones, optical gimbal feeds, intercept dispatch vectors, and direct bearing calculators.

### 2. Multi-Sector Radar Simulation
- **Northern Sector:** High-altitude Himalayan border corridor with extreme terrain masking.
- **Western Desert Corridor:** Low-altitude stealth intrusions and radar shadow corridors.
- **Eastern High-Altitude Pass:** Swarm drone vector incursions and electronic countermeasure zones.
- **Maritime Perimeter:** Coastal patrol corridors with surface vessel AIS data fusion.

### 3. High-Fidelity 3D Vehicle Models (Three.js)
- Real-time 3D rendered models for:
  - **UAV / Predator / Reaper class** drones
  - **Military Fighters / Interceptors** (Delta-wing supersonic jets)
  - **Commercial Airliners** (Twin-engine swept-wing cruisers)
  - **Unknown / Unidentified Aerial Targets** (Radar anomalies & evasive stealth crafts)
- Complete with scanline wireframes, studio key-lighting rigs, aerodynamic pitch/yaw/roll kinematics, and GPU memory-safe WebGL recursive cleanup.

### 4. Real-time Multi-Operator Satellite Chat
- **Dual-Mode Communication:**
  - **Tactical Hinglish AI Assistant:** Offline autonomous rule-based AI answering queries about aircraft vectors, radar jamming, simulation controls, and sector details.
  - **Supabase Realtime Satellite Broadcast:** Instant zero-latency cross-operator messaging across different laptops and mobile devices on the network.
- Floating draggable widget with Framer Motion spring physics, unread badges, and operator callsign identity customization.

### 5. Tactical Analytics & Audit Logging
- Live radar sweep metrics, track classification breakdown, and dynamic sector threat assessment.
- Full event detail dossiers with quick-jump **"Inspect in 3D"** deep-linking.
- Natural numerical and case-insensitive track sorting (`localeCompare`).

---

## 🛠️ Technology Stack

- **Frontend Core:** React 19, TypeScript, Vite 6
- **3D Graphics & Visualization:** Three.js, Canvas API
- **Animations & UI Physics:** Framer Motion
- **Styling:** Vanilla CSS, TailwindCSS v4 with tactical military chocolate/matte dark palette
- **Icons:** Lucide React
- **Cloud Backend:** Supabase (Postgres & Realtime WebSockets)
- **PWA Ready:** `vite-plugin-pwa` with offline caching & Service Worker

---

## 📦 Project Structure

```text
aegis-x/
├── public/
│   ├── advanced-console.html     # Standalone Deep 3D Tactical C2 Console
│   ├── favicon.svg               # Tactical vector logo
│   └── sw.js                     # Service Worker
├── src/
│   ├── components/
│   │   ├── 3d/                   # Three.js 3D aircraft models & viewers
│   │   ├── chat/                 # Floating tactical AI & Supabase chat
│   │   ├── dashboard/            # Main C2 layout & metrics
│   │   ├── events/               # Event dossier drawers & logs
│   │   ├── layout/               # TopBar, Modals, Callout Tips
│   │   ├── map/                  # Central tactical radar map & overlays
│   │   ├── pages/                # LiveTracksView, AnalyticsView, etc.
│   │   └── scenario/             # Sector selection modals
│   ├── context/
│   │   └── KshetraContext.tsx    # Global simulation state & kinematics
│   ├── types/
│   │   └── kshetra.ts            # TypeScript interfaces & types
│   ├── App.tsx                   # Main React entry point
│   └── index.css                 # Military tactical CSS styling system
├── vite.config.ts                # Vite config with manual chunk splitting
└── package.json                  # Dependencies & scripts
```

---

## ⚡ Getting Started Locally

### Prerequisites
- Node.js (v18.0.0 or higher recommended)
- npm or yarn

### 1. Installation
```bash
npm install
```

### 2. Development Mode
Run the local development server:
```bash
npm run dev
```
Open your browser at: `http://localhost:5173`

### 3. Production Build
Verify TypeScript compilation and bundle production assets:
```bash
npm run build
```
The optimized output will be in the `dist/` directory.

### 4. Preview Production Build
```bash
npm run preview
```

---

## 🌐 Deployment Instructions

### Option 1: Vercel (Recommended)
1. Push this codebase to your GitHub/GitLab repository.
2. Go to [Vercel Dashboard](https://vercel.com) and click **"New Project"**.
3. Import your repository.
4. Framework Preset: **Vite**.
5. Build Command: `npm run build`
6. Output Directory: `dist`
7. Click **Deploy**.

### Option 2: Netlify
1. Log in to [Netlify](https://netlify.com) and choose **"Add new site" > "Import an existing project"**.
2. Select your repository.
3. Build command: `npm run build`
4. Publish directory: `dist`
5. Click **Deploy Site**.

### Option 3: GitHub Pages / Static Hosting
1. Build the production bundle: `npm run build`
2. Deploy the `dist/` folder directly to GitHub Pages, Cloudflare Pages, AWS S3 / CloudFront, or any static web server.

---

## 🛡️ License & Classification

* **Classification:** SYNTHETIC SIMULATION ENVIRONMENT — DEFENSE LEVEL 4
* **Distribution:** Open for demonstration, evaluation, and operational training.
* Designed and built with high-fidelity tactical aesthetics for the modern defense battlespace.
