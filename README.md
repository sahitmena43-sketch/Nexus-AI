<div align="center">
  <h1>🤖 Nexus AI</h1>
  
  <p><strong>An intelligent Discord assistant — fast, accurate, and multilingual.</strong></p>
  
  <p>
    <a href="https://discord.com/oauth2/authorize?client_id=1547576998375858257">
      <img src="https://img.shields.io/badge/Invite%20Nexus%20AI-5865F2?style=for-the-badge&logo=discord&logoColor=white" alt="Invite Nexus AI">
    </a>
    <img src="https://img.shields.io/badge/Python-3.13-blue?style=for-the-badge&logo=python&logoColor=white" alt="Python 3.13">
    <img src="https://img.shields.io/badge/Gemini-Flash-orange?style=for-the-badge&logo=google&logoColor=white" alt="Gemini Flash">
    <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="MIT License">
  </p>
  
  <p>
    <a href="#-invite-nexus-ai">Invite</a> ·
    <a href="#-features">Features</a> ·
    <a href="#-commands">Commands</a> ·
    <a href="#-architecture">Architecture</a> ·
    <a href="#-privacy">Privacy</a> ·
    <a href="#-contributing">Contributing</a> ·
    <a href="#-license">License</a>
  </p>
</div>

---

**Nexus AI** is an intelligent Discord assistant built to help servers run better and give members fast, accurate answers to any question — in Albanian, English, or any other language.

Built on **Google Gemini** and **discord.py**, Nexus AI combines a powerful conversational assistant with dedicated tools for mathematics, web search, and server-aware knowledge.

---

## 🔗 Invite Nexus AI

Click the link below to add Nexus AI to your Discord server:

**👉 [Invite Nexus AI](https://discord.com/oauth2/authorize?client_id=1547576998375858257)**

Once invited, you can mention the bot directly or use its slash commands.

---

## ✨ Features

- 🤖 **Powerful AI assistant** — responds in Albanian, English, and any other language
- 🧮 **`/math` command** — solves any math problem step by step
- 🔍 **`/search` command** — scientific, social, sports, and general web search
- 💬 **`/ask` command** — free-form questions about anything Discord-related
- 🛡️ **Server-aware** — knows the channels, roles, and members of the server it is in
- 🌐 **Long responses** — sends replies up to 60,000 characters
- 🔄 **Automatic retry** — silently retries when the API is busy
- 🌍 **Multilingual** — replies in the same language the user writes in

---

## 📋 Commands

| Command | Description |
|---------|-------------|
| `/ask` | Ask a question about Discord |
| `/math` | Solve a math problem step by step |
| `/search` | Search for scientific, social, sports, and other information |
| `/model` | Change the AI model |

### How `/math` works

Solves any type of math problem:
- Arithmetic, algebra, geometry
- Trigonometry, calculus, statistics
- Probability and word problems

Shows all solution steps, not just the final answer.

### How `/search` works

Uses a multi-source search system with automatic fallback:

1. Tavily API
2. Brave Search API
3. SerpAPI
4. DuckDuckGo
5. Wikipedia

All citations are real sources — never fabricated.

---

## 🛠️ Architecture

Nexus AI stays lightweight by centering everything around a single loop: messages come in from Discord, the model decides whether extra tools are needed (web search, server knowledge), and the response is formatted and returned.

**Flow diagram:**
Discord User
│
▼
Nexus AI ──────► Google Gemini API
│
▼
Web Search
(Tavily, Brave,
SerpAPI,
DuckDuckGo,
Wikipedia)
│
▼
Formatted Response
│
▼
Discord User



### Tech Stack

- **Python 3.13** — main programming language
- **discord.py** — library for interacting with Discord
- **Google Gemini API** — the AI model (Gemini Flash)
- **aiohttp** — asynchronous HTTP requests
- **python-dotenv** — credential management
- **Pterodactyl** — hosting panel

### Project Structure
nexus-ai/
├── app.py # Main bot code
├── requirements.txt # Python dependencies
├── config.yaml # Configuration
├── .env # Credentials (not committed to Git)
└── README.md # This document



## 🔒 Privacy

- Credentials are stored in environment variables, not in code
- No personal information is stored
- All conversations are transient


## 🤝 Contributing

Nexus AI is an open project. If you'd like to contribute:

1. Open an **Issue** to report a bug or suggest a feature
2. Submit a **Pull Request** for a fix or new feature

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.


## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.


## 📞 Contact

For questions or suggestions, open an **Issue** in this repository.


<div align="center">
  <strong>Nexus AI</strong> — Your Discord assistant 🌍
  <br><br>
  <em>Thanks for visiting! ⭐</em>
</div>
