[README.md](https://github.com/user-attachments/files/31688697/README.md)
# 🧠 Why Did I Get It Wrong?

An AI-powered web app that analyzes math mistakes and explains exactly why a student's answer was wrong — step by step.

Built by **AbdulRahman Mohammed Abood** — Grade 9 student at Baghdad College High School, presented at the school's Research & Innovation Conference.

---

## 🎯 What It Does

Most tools just give you the correct answer. This app tells you **why your answer was wrong** — the exact step where your thinking went off track, and how to fix it.

You enter:
- The math question
- Your wrong answer
- The correct answer (optional)

The AI returns:
- ✅ The correct answer with full working
- ⚠️ The type of mistake (conceptual, arithmetic, sign error...)
- 📍 The exact point where it went wrong
- 🧠 Why your thinking was incorrect
- 📐 The correct approach step by step
- 💡 The key concept to remember
- 📝 3 similar practice problems to reinforce understanding

---

## ✨ Features

- **AI Error Analysis** — deep explanation of your specific mistake
- **14 Subjects** — Arithmetic, Algebra, Geometry, Trigonometry, Calculus, Statistics, Linear Algebra, Differential Equations, Number Theory, Combinatorics, Probability, Complex Analysis, Physics, Chemistry
- **AI Chatbot** — ask follow-up questions about the explanation after each analysis
- **Step-by-Step Mode** — solve problems step by step and get AI feedback on each step in real time
- **Mistake History** — every analysis is saved locally with weekly pattern reports
- **Spaced Repetition** — reminds you to review past mistakes you haven't revisited
- **Streak System** — tracks your daily practice streak
- **Built-in Calculator** — scientific calculator independent of the AI
- **Math Keyboard** — 50+ mathematical symbols for easy input
- **Export to PDF** — save any analysis as a printable PDF
- **Bilingual** — full Arabic and English support with academic-level output
- **3 Explanation Styles** — Simple, Normal, Technical
- **Dark & Light Mode**
- **Fully Responsive** — works on mobile, tablet, and desktop

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18, Tailwind CSS, HTML5 |
| Math Engine | Math.js (independent of AI) |
| AI Model | OpenAI GPT-OSS 120B via Groq API |
| Backend Proxy | Netlify Functions |
| Hosting | Netlify |

---

## 🚀 Getting Started

### Prerequisites
- A [Groq API key](https://console.groq.com) (free)
- A [Netlify](https://netlify.com) account (free)
- A [GitHub](https://github.com) account

### Folder Structure
```
why-did-i-get-it-wrong/
├── index.html
├── netlify.toml
└── netlify/
    └── functions/
        └── analyze.js
```

### Deploy to Netlify

1. Fork or clone this repo
2. Connect your GitHub repo to Netlify
3. Go to **Site Settings → Environment Variables**
4. Add a new variable:
   - Key: `GROQ_API_KEY`
   - Value: your Groq API key
5. Trigger a new deploy
6. Done ✅

The API key is never exposed in the frontend — all requests are proxied through a Netlify serverless function.

---

## 🔒 Security

The Groq API key is stored as a Netlify environment variable and injected server-side via a serverless function. It is never included in the frontend code or visible to users.

---

## 📸 Live Demo

🔗 [wdigiw-v2.netlify.app](https://wdigiw-v2.netlify.app)

---

## 📄 License

MIT — free to use, modify, and distribute.
