# ⚔️ QuestCraft – RPG Life Manager

> **Turn your daily tasks into an epic quest!**

QuestCraft is a gamified productivity web app that transforms your to‑do list into an RPG‑style adventure. Complete quests, earn coins, level up, maintain streaks, unlock achievements, and buy rewards — all in a beautiful dark glassmorphism interface.

---

## 🗺️ Features

- **Quest Map** – RPG‑style horizontal path with animated connectors. Max 12 active quests, up to 3 per category (Prime, Important, Urgent, Casual). Each quest rewards coins when completed.
- **Perish System** – Completed quests disappear after a smooth animation, freeing up slots for new adventures.
- **Shop** – Spend coins on rewards. Each reward costs a flat **40 coins** and **persists** after purchase — buy it as many times as you like!
- **Level & Streak** – Lifetime coins determine your level. A successful day (2+ Prime quests done) keeps your streak alive; two missed days reset it.
- **Statistics** – Weekly coin chart, category distribution, completion percentage, pending vs completed, and key metrics at a glance.
- **Achievements** – Unlock milestones (First Quest, 10/50/100 Quests, Level 10, 30‑day streak, etc.) with celebratory confetti.
- **Dashboard** – Overview of today's progress, active quests, coins, and level progress.
- **Settings** – Change your character, display name, export/import backup JSON, or reset all data.
- **Persistent Storage** – All data is saved in your browser's LocalStorage — no sign‑up, no backend required.

---

## 🛠️ Technology Stack

- **HTML5** – Semantic markup
- **CSS3** – Glassmorphism, animations, responsive design (desktop, tablet, mobile)
- **Vanilla JavaScript** – No frameworks, no dependencies. All logic in one file.

---

## 📦 Project Structure

```
QuestCraft/
└── index.html          # Single-file application (HTML + CSS + JS)
```

No build tools, no package managers — just open the file and play!

---

## 🚀 Getting Started

1. **Download** `index.html` from this repository.
2. **Double‑click** to open it in your favourite browser (Chrome, Firefox, Edge, etc.).
3. **Create your hero** – choose a character and enter a name.
4. **Start questing!** Add quests, complete them, earn coins, and build your legend.

All progress is saved automatically — come back anytime.

---

## 🎮 How to Play

### Quests
- Each quest belongs to one of four categories: **Prime (⭐)**, **Important (🔵)**, **Urgent (🔴)**, or **Casual (🟢)**.
- Prime quests award **40 coins**, Important **30**, Urgent **20**, Casual **10**.
- You can have up to **3 quests per category** and **12 total active quests**.
- To complete a quest, click its node on the map and hit **Complete**. The quest will disappear with a flourish, and you'll earn coins.

### Rewards
- Add rewards in the **Shop** (max 6 at a time).
- Every reward costs **40 coins**.
- Buying a reward does **not** remove it — you can purchase it again and again.
- Your purchase history is tracked for bragging rights.

### Streak
- To keep your streak alive, complete **at least 2 Prime quests** in a calendar day.
- One missed day = 1 strike. Two strikes in a row reset your streak to 0.

### Achievements
- Unlock achievements automatically as you progress (e.g., "First Quest", "Level 10 Champion", "100‑day Streak").
- A popup and confetti celebrate each new achievement.

---

## 🎨 Design

- **Dark Glassmorphism** – Frosted glass cards with subtle blur and border effects.
- **Accent Colours** – Purple, indigo, and gold for a premium, magical feel.
- **Responsive** – Adapts seamlessly from desktop to mobile.
- **Smooth Animations** – Everything from card hover to coin counters feels polished.

---

## 🔧 Customisation

All game parameters can be tweaked directly in the JavaScript:

- **Quest coin rewards** – modify the `getCategoryCoins()` function.
- **Reward cost** – change `return 40;` inside `getRewardCost()`.
- **Max quests per category** – adjust the `3` in the `addQuestBtn` validation.
- **Streak requirements** – alter the `2` in the streak evaluation logic.

---

## 🤝 Contributing

This is a single‑file project, but contributions are welcome!  
Feel free to fork, submit issues, or open pull requests for enhancements.

---

## 📄 License

MIT © 2026 – Free to use and modify.

---

## 🙏 Acknowledgements

Built with ❤️ and lots of coffee. Inspired by classic RPGs and gamified productivity apps.

---

**Start your quest today – every task is an adventure!** 🗡️🛡️
```
