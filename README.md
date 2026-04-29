# 🧠 Mental Health Chatbot — MAISH Hackathon 2024

> **🏆 3rd Place — MAISH Hackathon 2024**

A multilingual mental health support chatbot built to serve African-language speakers. Developed over 3 days — 2 days of building and a formal presentation day — under zero-budget constraints and without paid NLP APIs.

---

## 💡 The Problem

Mental health support resources in South Africa are largely English-only. Millions of people who are more comfortable expressing themselves in Zulu, Sotho, Tswana, or Venda are effectively excluded from digital mental health tools. This chatbot was built to close that gap.

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Language | JavaScript |
| NLP | Custom-built (no paid APIs) |
| Multilingual | Custom language detection engine |
| Conversation | Custom flow logic with fallback handling |

---

## ✨ Features

- **African Language Detection** — Identifies the user's language from input patterns and responds accordingly
- **Multi-language Response Mapping** — Responses available across multiple South African languages
- **Conversation Flow Logic** — Structured dialogue trees guiding users through check-ins and support prompts
- **Fallback Handling** — Graceful responses for unrecognised inputs, keeping the conversation going
- **Zero-budget Build** — No external APIs, no paid services — fully self-contained

---

## 🌍 Supported Languages

- English
- Zulu (isiZulu)
- (More to be added)

---

## 🔧 How It Works

```
User Input
    └── Language Detection Engine
            └── Identifies language from keyword patterns
            └── Selects appropriate response map
                    └── Conversation Flow Handler
                            └── Matches intent (greeting / check-in / support / crisis)
                            └── Returns contextual response
                            └── Fallback if unrecognised
```

### Language Detection (simplified logic)

```javascript
function detectLanguage(input) {
  const patterns = {
    zulu:    ['sawubona', 'yebo', 'ngiyabonga', 'unjani'],
    english: ['hello', 'hi', 'thanks', 'how are you']
  };
  // match input tokens against pattern lists
  // return detected language or default to english
}
```

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser
- No server required — runs client-side

### Run Locally

```bash
# Clone the repository
git clone https://github.com/NeoMudau/maish-chatbot.git
cd maish-chatbot

# Open in browser
open index.html
# or just drag index.html into your browser
```

---

## 📁 Project Structure

```
Sizwe-chatbot/
├── index.html              # Main UI
├── css/
│   └── styles.css          # Chatbot styling
├── js/
│   ├── app.js              # Entry point
│   ├── languageDetector.js # Language detection engine
│   ├── responseMap.js      # Language response mappings
│   └── flowHandler.js      # Conversation flow logic
└── README.md
```

---

## 🏆 Hackathon Context

**Event:** MAISH Hackathon 2024
**Result:** 3rd Place
**Format:** 3-day event — 2 days development, 1 formal presentation day
**Constraint:** Zero budget — no paid APIs or external services
**Team size:** [Add your team size here]

The challenge was to build a meaningful, working product from scratch and present it to a judging panel within 3 days. The chatbot was fully functional at presentation.

---

## 🔮 Future Improvements

- [ ] Add more South African languages (Xhosa, Ndebele, Tsonga)
- [ ] Integrate with a free NLP model for better intent detection
- [ ] Add crisis resource links per province (SADAG, suicide helplines)
- [ ] Build a backend to log anonymised session data for improvement
- [ ] PWA support for mobile access

---

## ⚠️ Disclaimer

This chatbot is not a substitute for professional mental health support. If you or someone you know is in crisis, please contact the **South African Depression and Anxiety Group (SADAG)** at **0800 456 789** (toll-free).

---

## 👤 Author

**Neo Pfarelo Mudau**
Full Stack Developer | JavaScript · Java · PHP · PostgreSQL

[LinkedIn](https://linkedin.com/in/codecraftedneo) · [GitHub](https://github.com/NeoMudau)
