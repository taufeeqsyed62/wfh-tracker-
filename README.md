# 🏠 WFH Tracker

A beautifully designed, single-file attendance tracker that helps you monitor your **Work From Home** vs **In-Office** days — with zero backend, zero dependencies, and persistent browser storage.

---

## ✨ Features

- 📅 **Interactive Calendar** — Navigate across any month, past or future
- 🏢 **Mark Attendance** — Click any weekday to log as *In Office* or *WFH*
- 📊 **Live Statistics** — Real-time percentage breakdown and animated progress bar
- 🚫 **Weekend Blocking** — Saturdays and Sundays are greyed out and non-selectable
- 💾 **Persistent Storage** — Data saved in `localStorage`; survives page reloads
- 📱 **Mobile Friendly** — Fully responsive design for all screen sizes
- 🎨 **Dark UI** — Sleek dark-mode interface with a modern aesthetic

---

## 🚀 Getting Started

No installation required. It's a single HTML file.

```bash
# 1. Clone or download the project
git clone https://github.com/your-username/wfh-tracker.git

# 2. Open the file in any browser
open wfh-tracker.html
```

Or simply double-click `wfh-tracker.html` — that's it.

---

## 🖱️ How to Use

| Action | How |
|---|---|
| Mark a day | Click any weekday on the calendar |
| Choose status | Select *In Office* 🏢 or *WFH* 🏠 from the popup |
| Clear a day | Click the day → select *Clear* |
| Navigate months | Use the `‹` and `›` arrows |
| Jump to today | Click the **Today** button |

### Example
If you mark **4 days as In Office** and **1 day as WFH**:
- **In Office:** 80%
- **WFH:** 20%
- **Total:** 5 days marked

The stats and progress bar update instantly.

---

## 📁 Project Structure

```
wfh-tracker/
└── wfh-tracker.html     # The entire app — HTML + CSS + JS in one file
```

No frameworks. No build tools. No npm. Just one file.

---

## 🗄️ Data Storage

All attendance data is stored in your browser's `localStorage` under the key:

```
wfh_tracker_data
```

Data is saved as a JSON object where each key is a date string and the value is the attendance type:

```json
{
  "2025-03-03": "office",
  "2025-03-04": "wfh",
  "2025-03-05": "office"
}
```

> ⚠️ Clearing your browser data or using a different browser/device will reset the tracker.

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Markup | HTML5 |
| Styling | CSS3 (custom properties, grid, flexbox, animations) |
| Logic | Vanilla JavaScript (ES6+) |
| Storage | Browser `localStorage` API |
| Fonts | Google Fonts — Syne + DM Sans |

---

## 📱 Browser Compatibility

Works on all modern browsers:

- ✅ Chrome / Edge
- ✅ Firefox
- ✅ Safari (desktop & iOS)
- ✅ Android Chrome

---

## 🎨 Customization

You can easily tweak the color scheme via CSS variables at the top of the `<style>` block:

```css
:root {
  --office: #00e5a0;   /* In-Office color */
  --wfh: #7b8cff;      /* WFH color */
  --bg: #0d0f14;       /* Background */
  --gold: #ffd166;     /* Accent / Today highlight */
}
```

---

## 📜 License

MIT License — free to use, modify, and distribute.

---

## 🙌 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

*Built with ❤️ as a single HTML file. No servers. No tracking. Your data stays in your browser.*
