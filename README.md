# 🚌 HK Bus Point-to-Point Tracker

Real-time Hong Kong bus tracker with **bookmarks** and **commute view**.

Track buses from your saved places (Home, Office, Gym, etc.) and instantly see which bus is coming next — sorted by remaining waiting time.

![HK Bus Tracker](https://raw.githubusercontent.com/KingsleyKwan/hk_bus_point_to_point_tracking/main/screenshot.png)

## ✨ Features

- **📌 10 Bookmarks** — Save any bus stop with a custom name
- **⏱ Live ETA** — Real-time arrival times from KMB/LWB official API
- **🚏 Commute View** — See next buses from "Home" sorted by wait time
- **🔍 Route Search** — Find any route and bookmark stops
- **📱 Mobile Friendly** — Works great on iPhone & Android
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

### 1. Add Bookmarks (Home, Office, etc.)

1. Open the app
2. Go to **Bookmarks** tab → click **+ Add Bookmark**
3. Search a route (e.g. `118`, `960`, `1A`)
4. Select direction/service
5. Choose a stop and give it a name (e.g. "Home", "Office")
6. Repeat for up to 10 places

### 2. Commute View (See Next Bus)

1. Go to **Commute View** tab
2. Select your **Home** bookmark
3. (Optional) Select your **Office** bookmark
4. The screen shows all incoming buses at your home stop, **sorted by shortest wait time**

This answers the question: *"What’s the next bus I can take from home?"*

### 3. Live Updates

- Bookmarks auto-refresh every 40 seconds
- Click any bookmark card to see full arrival list
- Pull-to-refresh works on mobile browsers

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

---

### Need Help?

Open an issue or contact the maintainer.