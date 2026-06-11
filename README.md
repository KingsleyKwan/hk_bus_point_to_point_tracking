# 🚌 HK Bus Point-to-Point Tracker

Real-time Hong Kong bus tracker with **bookmarks**, **commute view**, and **smart Point-to-Point** search.

**New:** At any plaza or stop with many bus options, select your "From" and "To" saved locations. The app now intelligently shows **only buses that actually stop at both** — sorted by shortest wait time. No more checking route-by-route!

![HK Bus Tracker](https://raw.githubusercontent.com/KingsleyKwan/hk_bus_point_to_point_tracking/main/screenshot.png)

## ✨ Features

- **📌 10 Bookmarks** — Save any bus stop with a custom name (Home, Office, Plaza, etc.)
- **🚏 Point-to-Point Search** — Select From + To → see **only direct buses** that serve both stops, sorted by wait time (solves the "many buses at one plaza" problem)
- **⏱ Live ETA** — Real-time arrival from official KMB/LWB API
- **🚏 Commute View** — Next buses from your Home bookmark
- **🔍 Route Search** — Find any route and bookmark stops
- **📱 Fully Mobile Optimized** — Excellent on iPhone & Android (larger selects, touch-friendly, auto-trigger)
- **🌐 Multi-language** — English / 繁體中文
- **⚡ Zero Build** — Just open `index.html`

## 🚀 Quick Start (Mobile)

### Option 1: GitHub Pages (Recommended)

1. Go to your repo: https://github.com/KingsleyKwan/hk_bus_point_to_point_tracking
2. Click **Settings → Pages**
3. Set **Source** to `Deploy from a branch`
4. Choose branch `main` and folder `/ (root)`
5. Click **Save**

After 30–60 seconds, your live URL will appear (e.g. `https://kingsleykwan.github.io/hk_bus_point_to_point_tracking/`).

Open this URL on your phone → **Add to Home Screen** for an app-like experience.

### Option 2: Netlify Drop (Fastest)

1. Go to https://app.netlify.com/drop
2. Drag the entire `hk-bus-tracker` folder into the browser
3. Get an instant public URL

### Option 3: Local Testing

```bash
cd hk-bus-tracker

# Python
python3 -m http.server 8080

# or Node
npx http-server -p 8080
```

Then open `http://localhost:8080` on your computer or phone (same Wi-Fi).

## 📖 How to Use

### 1. Add Bookmarks (Home, Office, Plaza, etc.)

1. Open the app
2. Go to **Bookmarks** tab → click **+ Add Bookmark**
3. Search a route (e.g. `118`, `960`, `1A`)
4. Select direction/service
5. Choose a stop and name it (e.g. "Festival Walk", "Home")
6. Repeat for your frequent locations (max 10)

**Tip:** Bookmark stops near plazas/malls you often use.

### 2. Point-to-Point Planner (Main New Feature)

1. Go to **Plan Trip** tab
2. Choose your current **FROM** location
3. Choose your **TO** destination
4. Tap **🔍 Find Direct Buses...**
5. Get a clean list of only the buses that go from From → To, **sorted by shortest wait time**

This solves the common pain point: "There are many buses here — which one actually goes where I need?"

### 3. Commute View

1. Go to **Commute View** tab
2. Select your **Home** bookmark
3. (Optional) Select your **Office** bookmark
4. See next buses at home, sorted by wait time

### 3. Point-to-Point (New Core Feature)

1. Add bookmarks for common locations (e.g. "Festival Walk", "Home", "Office")
2. Go to **Plan Trip** tab
3. Select **FROM** and **TO**
4. Tap **Find Direct Buses** — only routes that physically stop at both locations appear, sorted by shortest wait time

**Perfect for busy plazas where 10+ buses stop but only a few go where you need.**

### 4. Live Updates

- Bookmarks & Plan Trip auto-refresh
- All views update every 40 seconds
- Click any result for full details
- Fully touch-optimized for mobile browsers (add to Home Screen for app-like feel)

## 🗺 Data Source

All real-time data comes from the official Hong Kong government open data API:

- **KMB / LWB** — https://data.etabus.gov.hk
- No API key required
- Updates every 30–60 seconds

## 📁 Project Structure

```
hk-bus-tracker/
├── index.html          # Single-file app (all JS + Tailwind)
├── README.md
├── LICENSE
└── .gitignore
```

No `node_modules`, no build step, no package.json.

## 🛠 Development

Want to customize?

1. Edit `index.html`
2. Test locally with any static server
3. Commit and push — GitHub Pages updates automatically

## 📄 License

MIT License — feel free to use, modify, and deploy.

---

Built with ❤️ for Hong Kong commuters  
Data: Transport Department (HKSAR)  
Zero backend • Zero build • Works on any device

**Note**: The Tailwind CDN warning in browser console is expected for this single-file demo (production apps should use the CLI). It does not affect functionality.

---

### Need Help?

Open an issue or contact the maintainer.