<div align="center">

<img src="https://img.shields.io/badge/GrowthOS-v1.0.0-7c3aed?style=for-the-badge&logo=lightning&logoColor=white" />
<img src="https://img.shields.io/badge/Built%20With-Vanilla%20JS-f59e0b?style=for-the-badge&logo=javascript&logoColor=black" />
<img src="https://img.shields.io/badge/No%20Framework-Pure%20HTML%2FCSS%2FJS-2563eb?style=for-the-badge" />
<img src="https://img.shields.io/badge/Storage-LocalStorage-10b981?style=for-the-badge" />

<br/><br/>

```
   ██████╗ ██████╗  ██████╗ ██╗    ██╗████████╗██╗  ██╗ ██████╗ ███████╗
  ██╔════╝ ██╔══██╗██╔═══██╗██║    ██║╚══██╔══╝██║  ██║██╔═══██╗██╔════╝
  ██║  ███╗██████╔╝██║   ██║██║ █╗ ██║   ██║   ███████║██║   ██║███████╗
  ██║   ██║██╔══██╗██║   ██║██║███╗██║   ██║   ██╔══██║██║   ██║╚════██║
  ╚██████╔╝██║  ██║╚██████╔╝╚███╔███╔╝   ██║   ██║  ██║╚██████╔╝███████║
   ╚═════╝ ╚═╝  ╚═╝ ╚═════╝  ╚══╝╚══╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝
```

### **A personal productivity & self-growth dashboard built with pure HTML, CSS & JavaScript**
### *Track habits. Solve problems. Write daily. Level up your life.*

<br/>

[![Live Demo](https://img.shields.io/badge/⚡_Live_Demo-Try_Now-7c3aed?style=for-the-badge)](https://aryan150704.github.io/Growth-Os/GrowthOS.html)
&nbsp;
![Stars](https://img.shields.io/github/stars/Aryan150704/Growth-Os?style=for-the-badge&color=f59e0b)
&nbsp;
![License](https://img.shields.io/badge/license-MIT-2563eb?style=for-the-badge)
</div>

---

## 📌 What is GrowthOS?

**GrowthOS** is a fully dynamic, single-file personal productivity dashboard designed to make self-improvement measurable, visual, and motivating. Built entirely with **HTML5, CSS3, and vanilla JavaScript** — zero frameworks, zero dependencies you need to install, zero backend required.

It was built as a **portfolio-grade frontend project** to demonstrate:
- Complex JavaScript architecture with modular design
- Dynamic DOM rendering with real-time UI updates
- Data visualization using Chart.js
- Gamification mechanics (XP, levels, streaks)
- Responsive glassmorphism UI with dark theme
- LocalStorage-based data persistence

> *Open the file. No npm install. No build step. No server. Just open and go.*

---

## ✨ Feature Overview

| Module | What it does |
|---|---|
| 🏠 **Dashboard** | Daily productivity score ring, XP progress, greeting + motivational quote, habit & goal summary, activity feed |
| ✅ **Habit Tracker** | Add habits with emoji picker, one-click daily check-off, streak tracking, total completion count |
| 📔 **Daily Journal** | Mood selector (5 levels), free-text entry, custom tag system — all saved per day |
| 💻 **Coding Tracker** | Log DSA problems by topic + difficulty, XP per difficulty, top-topics breakdown, full problem history |
| 🎯 **Goals** | Goal cards with progress bars, deadline countdowns, auto-complete detection |
| 📊 **Analytics** | 4 live Chart.js charts — weekly XP, habit completion, coding by difficulty, 30-day activity trend |
| ⏱ **Pomodoro Timer** | Fully custom work/break durations, animated ring timer, auto phase switching, session log |
| 🗓 **Heatmap** | GitHub-style 53-week contribution grid, longest streak, active rate stats |

---

## 🎮 XP & Leveling System

Every action earns XP. Progress through **10 levels** as you build discipline.

```
✅ Complete a habit       → +10 XP
📔 Write a journal entry  → +15 XP
💻 Solve Easy problem     → +15 XP
💻 Solve Medium problem   → +25 XP
💻 Solve Hard problem     → +40 XP
🎯 Update goal progress   → +5–25 XP
🏆 Complete a goal        → +50 XP
⏱ Finish Pomodoro session → +20 XP
```

| Level | Title | XP Required |
|---|---|---|
| 1 | Beginner | 0 |
| 2 | Initiate | 150 |
| 3 | Consistent | 350 |
| 4 | Focused | 600 |
| 5 | Disciplined | 950 |
| 6 | Dedicated | 1,400 |
| 7 | Expert | 2,000 |
| 8 | Master | 2,800 |
| 9 | Elite | 3,800 |
| 10 | **Discipline Master** | 5,200 |

---

## 🛠 Tech Stack

```
Frontend        →  HTML5 · CSS3 · JavaScript (ES6+)
Charts          →  Chart.js 4.4
Icons           →  Font Awesome 6.5
Fonts           →  Syne (headings) · Outfit (body) — Google Fonts
Storage         →  Browser LocalStorage
Build Tools     →  None — single file, zero build step
```

**Key CSS techniques used:**
- Glassmorphism cards (`backdrop-filter: blur`)
- CSS custom properties for full theming
- Radial gradient nebula background
- SVG stroke-dasharray animated rings
- CSS keyframe animations for page transitions & toasts

**Key JS patterns used:**
- Module-like architecture with isolated render functions per page
- Observer-style sidebar sync after every XP change
- Global Pomodoro state object that persists across page navigation
- Chart.js instance management with destroy-on-navigate to prevent canvas leaks
- Dynamic DOM generation — zero static page content, everything rendered by JS

---

## 🚀 Getting Started

### Option 1 — Direct open (recommended)

```bash
# Clone the repo
git clone https://github.com/Aryan150704/GrowthOS.git

# Open in browser — that's it
open GrowthOS.html
```

### Option 2 — Local server (optional)

```bash
# Python
python -m http.server 3000

# Node
npx serve .
```

> Then visit `http://localhost:3000/GrowthOS.html`

**No npm. No package.json. No config files. Just one `.html` file.**

---

## 📁 Project Structure

```
GrowthOS/
├── GrowthOS.html          # The entire application (HTML + CSS + JS)
├── README.md              # You are here
└── exports/               # Optional: your exported JSON backups
    └── growthOS_YYYY-MM-DD.json
```

Everything lives in `GrowthOS.html`. The internal structure follows this pattern:

```
GrowthOS.html
├── <style>
│   ├── CSS Variables (dark theme tokens)
│   ├── Layout (sidebar + main grid)
│   ├── Component styles (cards, buttons, forms, badges)
│   └── Page-specific styles (heatmap, pomodoro ring, habits)
│
├── <body>
│   ├── #sidebar          (navigation + XP bar)
│   ├── #main             (8 page containers)
│   ├── #modal            (reusable modal overlay)
│   └── #toast-container  (XP gain notifications)
│
└── <script>
    ├── DB helpers         (getDB / saveDB via localStorage)
    ├── XP system          (addXP, getLevelProgress)
    ├── Navigation         (go(), page renderer dispatch)
    ├── renderDash()       (dashboard page)
    ├── renderHabits()     (habits CRUD + toggle)
    ├── renderJournal()    (journal with mood + tags)
    ├── renderCoding()     (DSA tracker)
    ├── renderGoals()      (goal management)
    ├── renderAnalytics()  (Chart.js integration)
    ├── renderPomo()       (timer state machine)
    ├── renderHeatmap()    (52-week grid generation)
    └── exportJSON()       (data export)
```

---

## 📊 Data Schema

All data is stored in `localStorage` under the key `growthOS_v3`.

```json
{
  "user": {
    "name": "Your Name",
    "xp": 540
  },
  "habits": [
    {
      "id": "abc123",
      "name": "Morning meditation",
      "emoji": "🧘",
      "completedDates": ["2025-05-28", "2025-05-29"],
      "createdAt": "2025-05-01"
    }
  ],
  "journal": [
    {
      "id": "def456",
      "date": "2025-05-29",
      "mv": 4,
      "me": "🙂",
      "ml": "Good",
      "text": "Had a productive day solving DP problems.",
      "tags": ["leetcode", "focused"]
    }
  ],
  "coding": [
    {
      "id": "ghi789",
      "title": "Longest Palindromic Substring",
      "diff": "Medium",
      "topic": "Dynamic Programming",
      "time": 35,
      "date": "2025-05-29",
      "xp": 25
    }
  ],
  "goals": [
    {
      "id": "jkl012",
      "title": "Solve 150 LeetCode Problems",
      "target": 150,
      "cur": 42,
      "deadline": "2025-08-01",
      "done": false
    }
  ],
  "pomo": {
    "work": 25,
    "brk": 5,
    "sessions": []
  },
  "log": [
    {
      "date": "2025-05-29",
      "type": "coding",
      "desc": "Solved Medium: Two Sum",
      "xp": 25
    }
  ]
}
```

---

## 💾 Export & Backup

Click **"Export Data (JSON)"** in the sidebar footer to download a timestamped backup of all your data:

```
growthOS_2025-05-29.json
```

You can re-import it later by opening the browser console and running:

```javascript
localStorage.setItem('growthOS_v3', JSON.stringify(/* paste JSON here */));
location.reload();
```

---

## 🖼 UI Design Decisions

| Decision | Reasoning |
|---|---|
| **Dark theme only** | Reduces eye strain for long coding sessions; matches developer aesthetic |
| **Glassmorphism cards** | Creates depth and modern feel without heavy CSS overhead |
| **Purple + Blue palette** | High contrast against dark bg; energetic without being harsh |
| **Syne font (headings)** | Angular, futuristic — matches the productivity-system vibe |
| **SVG rings (not canvas)** | Lightweight, CSS-animatable, scalable at any DPI |
| **Single HTML file** | Maximum portability — works offline, on any device, no setup |
| **No framework** | Demonstrates raw JS ability; faster load; simpler to understand and fork |

---

## 🔮 Planned Improvements

- [ ] PWA support (offline-first with Service Worker)
- [ ] Import JSON data back into the app
- [ ] Drag-and-drop habit reordering
- [ ] Keyboard shortcuts (`H` → Habits, `J` → Journal, etc.)
- [ ] Weekly review summary auto-generated from journal entries
- [ ] Dark/light theme toggle
- [ ] Mobile bottom navigation bar
- [ ] Notification reminders via Web Notifications API
- [ ] Cloud sync via Firebase (optional backend upgrade)

---

## 🤝 Contributing

This is a personal portfolio project, but PRs and suggestions are very welcome!

```bash
# Fork the repo, then:
git checkout -b feature/your-feature-name
# Make your changes to GrowthOS.html
git commit -m "feat: add your feature"
git push origin feature/your-feature-name
# Open a Pull Request → https://github.com/Aryan150704/GrowthOS
```

Please keep contributions to the **single-file architecture** unless there's a very strong reason to split.

---

## 📄 License

```
MIT License — feel free to fork, modify, and use in your own projects.
Credit appreciated but not required.
```

---

<div align="center">

**Built with obsession, caffeine, and a deep belief that consistency compounds.**

*If this project helped you or impressed you — drop a ⭐ on the repo. It means a lot.*

<br/>

![Made with HTML](https://img.shields.io/badge/Made%20with-HTML5-e34f26?style=flat-square&logo=html5&logoColor=white)
![Made with CSS](https://img.shields.io/badge/Made%20with-CSS3-1572b6?style=flat-square&logo=css3&logoColor=white)
![Made with JS](https://img.shields.io/badge/Made%20with-JavaScript-f7df1e?style=flat-square&logo=javascript&logoColor=black)

</div>
