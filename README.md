# 🐢 KIRA × Turtlesim

![HTML](https://img.shields.io/badge/HTML-CSS-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Groq](https://img.shields.io/badge/Groq-LLaMA_3.3_70B-FF6B35?style=for-the-badge)
![Vercel](https://img.shields.io/badge/Deployed-Vercel-000000?style=for-the-badge&logo=vercel)
![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=for-the-badge)

A browser-based turtle simulator integrated with **KIRA** — an expressive AI companion powered by Groq's LLaMA 3.3 70B. Navigate the turtle by clicking on the canvas or using voice commands, while KIRA responds to your speech, reacts with animated emotions, and speaks back in real time.

---

## 🌐 Live Demo

> [**Try it live →**](https://kira-turtle-deploy.vercel.app)

---

## ✨ Features

- **🐢 Turtle Simulator** — Click anywhere on the grid to set a navigation target; the turtle autonomously pathfinds to it
- **🎙️ Voice Control** — Speak commands (`forward`, `back`, `left`, `right`, `stop`) to control the turtle hands-free
- **🤖 KIRA AI Companion** — Powered by Groq's LLaMA 3.3 70B; responds conversationally to anything you say
- **😊 Animated Emotions** — KIRA's SVG face changes expression in real time (happy, thinking, excited, listening, neutral)
- **🔊 Speech Synthesis** — KIRA speaks her responses back to you using the browser's Web Speech API
- **✍️ Trail Drawing** — The turtle draws a glowing trail as it moves across the canvas

---

## 🧠 How It Works

```
Voice Input (Web Speech API)
        ↓
  Movement command? → Control turtle directly (forward/back/left/right/stop)
  Conversation?     → Send to Groq API (LLaMA 3.3 70B)
                              ↓
                      KIRA responds + sets emotion tag
                              ↓
                      Display in chat + Speak response
```

When the turtle reaches a clicked target, KIRA automatically narrates the arrival and prompts for the next action.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, JavaScript (Vanilla) |
| AI Model | LLaMA 3.3 70B via Groq API |
| Voice Input | Web Speech API (SpeechRecognition) |
| Voice Output | Web Speech API (SpeechSynthesis) |
| Rendering | HTML5 Canvas |
| Deployment | Vercel |

---

## 🚀 Getting Started

### Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/Ashritha-Abbabathula/kira-turtle-deploy.git
   ```
2. Open `index.html` in your browser — no build step needed
3. Enter your [Groq API key](https://console.groq.com) when prompted
4. Start talking to KIRA!

### Get a Groq API Key
1. Sign up at [console.groq.com](https://console.groq.com)
2. Go to **API Keys** → **Create API Key**
3. Paste it when prompted on first load
4. Your key is saved locally in `localStorage` — never shared

---

## 🎮 Controls

| Action | How |
|--------|-----|
| Set navigation target | Click anywhere on the canvas |
| Move forward | Say **"forward"** |
| Move backward | Say **"back"** |
| Turn left | Say **"left"** |
| Turn right | Say **"right"** |
| Stop | Say **"stop"** |
| Talk to KIRA | Say anything else |
| Update API key | Click **RESET API KEY** (top right) |

---

## 📁 File Structure

```
kira-turtle-deploy/
├── index.html        # Entire app — simulator + KIRA UI + logic
└── README.md
```

---

## 👩‍💻 Author

**Ashritha Abbabathula**  
[![GitHub](https://img.shields.io/badge/GitHub-Ashritha--Abbabathula-181717?style=flat&logo=github)](https://github.com/Ashritha-Abbabathula)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
