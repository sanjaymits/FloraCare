# 🌿 Verdant Care — AI Plant App

A Progressive Web App (PWA) for plant identification, health diagnosis, and watering schedules — powered by Claude AI.

## Features
- 📸 **Identify plants** by photo using AI
- 🩺 **Diagnose plant health** from images + symptoms
- 💧 **Watering schedules** and care instructions
- 📱 **iPhone installable** — works like a native app

---

## Deploy to Vercel

### 1. Install Vercel CLI
```bash
npm install -g vercel
```

### 2. Set up your Anthropic API Key
Go to [console.anthropic.com](https://console.anthropic.com) to get your API key.

### 3. Deploy
```bash
cd verdant-care
vercel
```

When prompted, add your environment variable:
```
ANTHROPIC_API_KEY = your_key_here
```

Or set it in the Vercel dashboard under **Settings → Environment Variables**.

### 4. Install on iPhone
1. Open your deployed URL in **Safari**
2. Tap the **Share** button (box with arrow)
3. Tap **"Add to Home Screen"**
4. Tap **"Add"**

Verdant Care will appear on your home screen like a native app! 🌿

---

## Project Structure
```
verdant-care/
├── index.html          # My Garden (home screen)
├── identify.html       # AI Plant Identifier
├── diagnosis.html      # AI Health Diagnosis
├── plant-detail.html   # Plant Care Details
├── api/
│   ├── identify.js     # Serverless: plant ID endpoint
│   └── diagnose.js     # Serverless: diagnosis endpoint
├── service-worker.js   # PWA offline support
├── manifest.json       # PWA configuration
├── vercel.json         # Vercel routing config
└── icon-192.svg        # App icon
```

---

## Local Development
```bash
npm install -g vercel
vercel dev
```
Then open `http://localhost:3000`
