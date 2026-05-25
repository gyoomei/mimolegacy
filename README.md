# 🌟 MiMoLegacy

### AI Wisdom Vault — Powered by Xiaomi MiMo V2.5

Capture hard-earned life lessons. Transform raw experience into timeless advice cards. Share wisdom across generations.

[![Live Demo](https://img.shields.io/badge/Live-Demo-000?style=for-the-badge&logo=github)](https://gyoomei.github.io/mimolegacy/)
[![Try Now](https://img.shields.io/badge/Try-Now-e8a838?style=for-the-badge&logo=googlechrome)](https://gyoomei.github.io/mimolegacy/)
[![AI](https://img.shields.io/badge/AI-Xiaomi%20MiMo%20V2.5-f97316?style=for-the-badge)](https://huggingface.co/XiaomiMiMo)
[![Domains](https://img.shields.io/badge/Domains-6%20Life%20Areas-8b5cf6?style=for-the-badge)](#the-6-life-domains)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

---

## 📖 The Problem

We accumulate thousands of life lessons — from career failures, financial mistakes, relationship breakthroughs, health scares. But wisdom stays trapped in our heads. It dies with us. Our children repeat the same mistakes because we never articulated what we learned in a way that sticks.

**MiMoLegacy fixes that.** Describe a raw experience. MiMo V2.5 distills it into a polished, universal piece of wisdom — written like advice from a wise elder, stored in your personal vault, ready to share.

---

## ✨ How it works

```
You write:    "I learned that saving 30% of income from day one matters
               more than any investment trick. After going broke twice."

MiMo writes:  "The most powerful investment strategy isn't a stock pick
               or a crypto bet — it's the discipline of setting aside
               30% before you learn what you're missing. Future you will
               thank present you for the boring, unglamorous habit of
               paying yourself first."
```

**That's the entire UX** — write, transform, preserve, share.

---

## 🎯 Core Features

| Capability | Detail |
|---|---|
| 🧠 **AI Wisdom Distiller** | Raw experience → polished advice in second-person "wise elder" voice |
| 💼 **6 Life Domains** | Career · Finance · Relationship · Health · Parenting · General |
| 📚 **Personal Vault** | Save up to 50 wisdom cards to localStorage |
| 📊 **Stats Dashboard** | Track wisdom by domain, weekly capture rate, category breakdown |
| 💬 **Reflect with MiMo** | Chat companion for deeper reflection on experiences and saved wisdom |
| 🎨 **Card Themes** | Copy wisdom cards with one click |
| 🔍 **Filter & Search** | Browse vault by life domain |
| 🌗 **Dark/Light Mode** | Warm amber + midnight palette, WCAG-AA compliant |
| 🌐 **Bilingual EN/ID** | Full Indonesian + English translation |
| 📱 **Mobile Responsive** | Fluid from 375px to 1920px |
| 🔁 **Retry Logic** | 3-attempt fetch with graceful fallback |
| 🫧 **Atmospheric UI** | Drifting orbs, rising particles, grid overlay |

---

## 🔮 The 6 Life Domains

| Domain | Icon | Best for |
|---|---|---|
| 💼 **Career** | Professional growth | "After 10 years in tech, I learned..." |
| 💰 **Finance** | Money & wealth | "Going broke taught me that..." |
| ❤️ **Relationship** | Love & connection | "The hardest lesson about love was..." |
| 🧘 **Health** | Body & mind | "Ignoring burnout cost me..." |
| 👶 **Parenting** | Raising children | "What I wish I knew before becoming a parent..." |
| 🌍 **General** | Life philosophy | "The older I get, the more I realize..." |

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│  Input: Raw lesson + Domain + Context                       │
│                          ↓                                   │
│  Prompt Builder           →  domain-specific system prompt   │
│  (6 domain templates)        with "wise elder" voice         │
│                          ↓                                   │
│  MiMo V2.5 (Pollinations.ai) → polished advice text          │
│                          ↓                                   │
│  Wisdom Card Renderer     →  styled card with metadata       │
│                          ↓                                   │
│  Vault (localStorage)     →  save, filter, share             │
│                          ↓                                   │
│  Stats Engine             →  domain breakdown + analytics    │
└─────────────────────────────────────────────────────────────┘
```

**Zero backend.** Everything runs client-side in your browser. No API key. No tracking.

---

## 💡 Architecture Decisions

**Why single HTML?**
Zero deploy friction, zero backend cost, easy to fork. One file = one commit = one deploy. Anyone can clone and self-host in one minute.

**Why client-side only?**
Privacy. Your deepest life lessons stay in YOUR browser. Nothing hits a server we control. Wisdom is personal — it should stay that way.

**Why MiMo V2.5?**
Free via Pollinations.ai. No API key needed. Strong narrative reasoning — understands the "wise elder" voice, universal distillation, and the difference between raw experience and actionable advice.

**Why "wise elder" voice?**
Second-person advice written as if from someone who has lived many lives creates psychological weight. It transforms "I learned X" into "You will discover X" — making it feel like inherited wisdom, not personal complaint.

---

## 🧪 Try these examples

| Raw Input | Domain | Polished Wisdom |
|---|---|---|
| "Saving 30% from day one beats any trick" | Finance | The most powerful strategy is paying yourself first |
| "Promoted too fast, burned out in 6 months" | Career | Growth without foundation collapses under its own weight |
| "Said sorry first even when not wrong" | Relationship | The strongest bridges are built by those willing to cross first |
| "Skipped sleep for a year, body gave up" | Health | Your body keeps a ledger — every debt is eventually called |
| "Let kids fail small so they don't fail big" | Parenting | Controlled falls teach better than perfect protection |
| "Not every battle deserves your energy" | General | Wisdom is knowing which storms to weather and which to watch |

---

## 🛠️ Stack

- **Frontend:** Vanilla JavaScript, single HTML file (~40KB)
- **AI:** [Xiaomi MiMo V2.5](https://github.com/XiaomiMiMo) via [Pollinations.ai](https://text.pollinations.ai/) — free, no API key
- **Fonts:** [Sora](https://fonts.google.com/specimen/Sora) + [Nunito](https://fonts.google.com/specimen/Nunito) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono)
- **Storage:** localStorage for wisdom vault
- **Hosting:** GitHub Pages (zero infra cost)

---

## 🚀 Quick Start

```bash
git clone https://github.com/gyoomei/mimolegacy.git
cd mimolegacy
python3 -m http.server 8080
# Open http://localhost:8080
```

Or just visit the [live demo](https://gyoomei.github.io/mimolegacy/).

---

## 📄 License

MIT — capture your wisdom, share it freely.

---

**Built with 🧠 [Xiaomi MiMo V2.5](https://github.com/XiaomiMiMo) · Submitted to the [Xiaomi MiMo 100T program](https://100t.xiaomimimo.com/)**
