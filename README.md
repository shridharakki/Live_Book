# 📖 Living Textbook

> **A personalised AI tutor that lives inside your PDF — and remembers you.**

Most AI tools forget you the moment you close the tab. **Living Textbook is different.**  
It learns who you are, what you struggle with, and what you already know — building a personalised learning experience that gets smarter every time you return.

---

## 🎯 The Problem It Solves

Generic AI chatbots give the same answer to everyone.  
Living Textbook gives **your** answer — tailored to your learning history, your weak areas, and exactly where you left off.

---

## ✨ Key Features

| Feature | Description |
|--------|-------------|
| 📄 **PDF Reader** | Upload any textbook, article, or notes as a PDF |
| 🧠 **Personalised Explanations** | AI adapts its answers based on your past struggles and strengths |
| 📝 **Smart Quizzes** | Harder questions on your weak areas, easier on what you know well |
| 🔴 **Weak Area Tracker** | See exactly what needs revision — pulled from memory |
| ✅ **Progress Review** | Full learning history across all your sessions |
| 💬 **Highlight to Ask** | Select any text on the page and instantly ask the AI |
| 🌙 **Dark Mode** | Easy on the eyes for long study sessions |

---

## 🧩 How Personalisation Works

Living Textbook uses **[Backboard](https://app.backboard.io)** to power persistent memory across sessions.

- **First visit** — The AI introduces itself, learns your name, and notes your starting point
- **Every session** — The AI silently stores what you understood, what confused you, and which pages you studied
- **Return visits** — The AI greets you by name, reminds you where you left off, and adjusts its teaching style based on your history

> *"You found this concept tricky last time — let's break it down differently."*  
> *"You already understand this well, so let's build on it."*

This is not a generic chatbot. This is a tutor that **knows you**.

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | Vanilla HTML, CSS, JavaScript (zero dependencies) |
| PDF Rendering | PDF.js |
| AI Memory & Conversations | [Backboard](https://app.backboard.io) |
| Underlying LLM | GPT-4o mini (via Backboard) |

---

## 🧩 Backboard Features Used

| Feature | Purpose |
|--------|---------|
| **Persistent Memory** | Stores each student's struggles, strengths, and progress using `memory: 'Auto'` on every message |
| **Assistant** | Holds the personalised tutor system prompt and persona |
| **Thread** | Manages the conversation session — reused across visits so context is never lost |

---

## ⚙️ Getting Started

### Prerequisites
- A free Backboard API key → [app.backboard.io](https://app.backboard.io)
- Any modern browser (Chrome, Firefox, Edge, Safari)
- No installs. No build step. No server.

### Run Locally

```bash
git clone https://github.com/yourusername/living-textbook.git
cd living-textbook
```

Then simply open `index.html` in your browser.

### First Launch

1. Enter your **Backboard API key** when prompted
2. Upload any **PDF** on the left panel
3. Start learning — the AI will remember everything from this point forward ✅

---

## 📁 Project Structure

```
living-textbook/
└── index.html        # Entire app in a single file — no frameworks, no build tools
```

---

## 🔐 Privacy

- Your API key is stored only in your browser's `localStorage`
- No data is sent to any server other than Backboard (for memory and AI responses)
- Each user's memory is scoped to their own API key

---

## 📄 License

MIT — free to use, fork, and build upon.

---

<p align="center">Built with ❤️ to make learning more enjoyable and engaging..</p>
