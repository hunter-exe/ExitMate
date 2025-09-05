# ExitMate

**ExitMate** is a mobile app (React Native + Expo) that uses your device’s location and camera/mic permissions to enable practical, real-world workflows—like meeting/venue check-ins, geofenced actions, and quick “I’m on my way” sharing. It’s built to be fast to start locally, easy to test on a phone, and simple to deploy.

> TL;DR: Open the app, grant location permissions, and try the demo flows. Optional Node/Express backend included for APIs, persistence, and auth.

---

## ✨ Features
- 📍 **Location-aware** flows (foreground permissions; background optional)
- 🧭 **Geofenced** checks & simple rules (enter/exit area → action)
- 🔗 **Shareable session links** (optional, via backend)
- ⚡ **Instant dev run** on a physical device (Expo)
- ☁️ **Backend API** (optional) for users/rooms/sessions

---

## 🧱 Tech Stack
- **Mobile:** React Native + Expo (+ expo-router if used)  
- **Backend (optional):** Node.js + Express (+ Socket/WebSocket if used)  
- **Storage (optional):** any (e.g., MongoDB/SQLite/Postgres)  
- **Build/Dev:** Expo CLI, Metro bundler  
- **Deployment:** Expo (EAS) for mobile; Render/any Node host for backend

---

## ✅ Prerequisites
- **Node.js ≥ 18** (LTS recommended)
- **Package manager:** `npm` or `pnpm` or `yarn`
- **Expo CLI:** `npm i -g expo` (or use `npx expo`)
- **Expo Go** app on your phone (from Play Store / App Store)
- (Optional) **Backend** runtime (Node) and DB if you enable server features

---

## 🚀 Quick Start (Mobile App)

```bash
# 1) Clone
git clone https://github.com/hunter-exe/ExitMate.git
cd ExitMate

# 2) Install (inside the app directory)
# If your app sits in a subfolder, cd into it first (e.g., cd ExitMate)
npm install            # or pnpm install / yarn

# 3) Configure env (optional)
# If there is an .env.example, copy it:
# cp .env.example .env
# Fill keys described below.

# 4) Run in development (QR appears in terminal)
npm run start          # or npx expo start
