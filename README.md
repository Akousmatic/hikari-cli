# Hikari CLI - A Terminal Based Roleplay.

Elegant, fast CLI assistant with persistent memory, web search, all on your Terminal.

---

## Quick Start (Windows PowerShell)

1) Install dependencies
```powershell
python -m pip install -r requirements.txt
```

2) Configure API keys
```powershell
copy .env.example .env
# Edit .env and set:
# DEEPSEEK_API_KEY=your_deepseek_api_key
# BRAVE_API_KEY=your_brave_api_key
```

3) Start the CLI
```powershell
Hikari
```
4) Exit the CLI
```powershell
 /exit
```

## Commands
```powershell
/memory_stats - It shows how many conversations have been saved.
/exit - Exits the CLI shell.
hikari  --help - Shows commnds (some might be older commands that i forgot to remove from the help directory lol. you can help me remove them if you want
or you can try them if they work or don't.)
/usage - Shows how much token you have used, how many calls to the API and the costs.
```

---

## Features

- Persistent memory with auto‑summarization
- Clean 80‑column UI (no emojis in output), progress bars, syntax highlighting
- Real‑time web search via Brave Search (async)
- Safe file writes with confirmation prompts
- Multiple LLM support (eg; DeepSeek, OpenAI, Grok, Gemini)


---

## Configuration Notes

- Keep keys in .env; never hardcode secrets.
- Brave search is used automatically for “current/latest/today”-type queries; use --search to force it.
- All network and file operations include error handling and clear status messages.

---

## Troubleshooting

- Missing typer/rich/httpx: run requirements install again.
- API key errors: check .env and run `python main.py config`.
- Windows PowerShell only: commands above are PowerShell‑ready.

---

Status: Actively maintained; interactive shell, web search, and memory verified as of 2025‑09‑06.

### Future RoadMap:

- Voice to Voice with hot swappable-like 3d Anime models (like grok, bella)
- Custom Fine-Tuned Voice model.
- Sandbox - So it only generates functionable, tested scripts.
- Maybe a feature that scrapes anything from the web while continously self-improving to scrape your desired data.
- Discord integration.
