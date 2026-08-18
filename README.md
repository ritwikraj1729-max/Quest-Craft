# QuestCraft - Neural Mission Control

> Turn your daily tasks into a futuristic mission-control system.

QuestCraft is a gamified productivity web app that transforms your to-do list into a JARVIS-inspired, holographic command center. Resolve objectives, earn credits, rank up, maintain streaks, unlock honors, and buy rewards from a dark glassmorphism HUD with a cosmetic AI core.

---

## Features

- **Neural Mission Control UI** - Futuristic HUD with cyan/blue accents, glowing borders, animated particle field, grid overlay, scanlines, circular progress rings, and smooth micro-interactions.
- **Task Array (Right Sidebar)** - Collapsable floating tech cards grouped by priority (Prime, Important, Urgent, Casual). Clicking anywhere on a card completes the objective; hover for edit/delete. Max 12 active quests, up to 3 per category.
- **Requisitions (Left Sidebar)** - Collapsable floating tech cards for rewards (max 6). Acquire rewards with credits; every purchase is logged in the acquisition log.
- **Sidebar Nav** - The Command, Core Config, Calendar, Honors, and XP & Rank buttons live inside the sidebars to save space. Collapsed sidebars shrink to a slim strip with a re-expand button.
- **Neural Core (Center)** - The orb takes the whole center space. It sweeps, pulses, and bursts on interaction. Surrounding readouts show rank, credits, streak, and honors. Click it to open the neural-link console.
- **Floating HUD Readouts** - Progress and statistics float as small transparent displays on each side of the orb - compact weekly credit chart, lifetime completion ring, category completion, and key metrics. No panel headings, no scrolling.
- **Transparent Sidebars** - The sidebars have a transparent background, letting the particle field and grid shine through.
- **Cosmetic AI Core** - A purely visual "J.A.R.V.I.S." orb that reacts to clicks, task completion, XP gains, level-ups, and navigation. It opens a neural-link console with scripted, typewriter-style responses. No real AI, no chatbot, no LLM, no network calls.
- **Perish System** - Completed quests vanish with a smooth animation, freeing slots for new objectives.
- **Rank & Streak** - Lifetime XP determines your rank. A successful day (2+ Prime quests done) keeps your streak alive; two missed days reset it.
- **Honors (Achievements)** - Unlock milestones (First Directive, 10/50/100 Quests, Rank 10, 30-day streak, etc.) with celebratory confetti.
- **Calendar** - Month view marking the days you completed objectives.
- **Persistent Storage** - All data is saved in your browser's LocalStorage - no sign-up, no backend required.

---

## Technology Stack

- **HTML5** - Semantic markup
- **CSS3** - Glassmorphism, animated HUD, responsive layout
- **Vanilla JavaScript** - No frameworks, no dependencies, single-file app
- **Canvas** - Lightweight particle background

---

## Getting Started

1. Open `index.html` in your favourite browser (Chrome, Firefox, Edge, etc.).
2. Select an operative class and enter a callsign to establish the link.
3. Deploy objectives, complete them, earn credits, and rank up.

All progress is saved automatically - come back anytime.

---

## How It Works

### Objectives
- Each quest belongs to one of four priority classes: **Prime**, **Important**, **Urgent**, or **Casual**.
- Prime quests award **40 credits**, Important **30**, Urgent **20**, Casual **10**.
- Up to **3 quests per category** and **12 total active quests**.
- Complete a quest by clicking its card in the Task Array to earn credits and clear the slot.

### Rewards
- Add rewards in the Requisitions sidebar (max 6 at a time).
- Every reward costs **40 credits**.
- Buying a reward does not remove it - you can acquire it again.
- Purchase history is tracked in the acquisition log.

### Streak
- Complete at least **2 Prime quests** in a calendar day to keep the streak alive.
- One missed day = 1 strike. Two strikes in a row reset the streak.

### Honors
- Honors unlock automatically as you progress.
- A popup and confetti celebrate each new honor.

### AI Core
- The large orb at the center of the screen is the neural link. Click it to open the console.
- Try directives like `status`, `scan`, `sync`, `ping`, `objective <text>`, `help`, or `clear`.
- It is intentionally cosmetic - a visual simulation with canned responses, no real intelligence.

---

## Design

- **Dark Glassmorphism** - Frosted glass panels with blur and glow; sidebars are fully transparent.
- **Cyan / Blue Accents** - Futuristic HUD palette with gold highlights for credits and honors.
- **Mission Layout** - The neural orb fills the center; progress and statistics float as small transparent readouts on its sides. Left/right sidebars hold tasks, rewards, and nav buttons. On smaller screens, everything stacks and scrolling is allowed.
- **Smooth Animations** - GPU-friendly transforms, glow pulses, core bursts, and status sweeps.
- **Reduced Motion** - Respects the `prefers-reduced-motion` system setting.

---

## Customisation

All game parameters can be tweaked directly in the JavaScript:

- **Quest credit rewards** - modify the `getCategoryCoins()` function.
- **Reward cost** - change `return 40;` inside `getRewardCost()`.
- **Max quests per category** - adjust the `3` in `handleAddQuest()` validation.
- **Streak requirements** - alter the `2` in the streak evaluation logic.
- **Expand overlays** - edit the `EXP_MODULES` map and the `render*Overlay()` functions.
- **Achievement definitions** - edit the `ACHIEVEMENT_DEFS` array.

---

## License

MIT - Free to use and modify.
