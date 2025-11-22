# Shit-Post-Bot

An **automatic content downloader and re-uploader** designed to aggregate and redistribute humorous or viral media while avoiding duplicate content and targeting specific Facebook pages or keywords.

## 🧩 Features

- **Facebook Page & Keyword Targeting** — Define target sources and keywords in `config/targets.json`.
- **Duplicate Detection** — Uses perceptual hashing (image/text) to avoid reposting duplicate content.
- **Automatic Upload Scheduler** — Periodically uploads new content to designated destinations.
- **Extensible Source System** — Easily add new content sources or destinations.

## ⚙️ Project Structure

```
Shit-Post-Bot/
│
├── src/
│   ├── downloader.py      # Handles content fetching from Facebook and other APIs
│   ├── uploader.py        # Handles posting and upload scheduling
│   ├── dedupe.py          # Detects duplicates using hashes and similarity metrics
│   ├── utils.py           # Shared helper functions
│
├── config/
│   ├── targets.json       # List of Facebook pages and keyword filters
│   └── config.py          # Token management and runtime configuration
│
├── main.py                # Entrypoint for orchestrating the pipeline
│
└── requirements.txt       # Project dependencies
```

## 🔧 Setup

1. Clone the repo:
   ```bash
   git clone https://github.com/Nivek-C94/Shit-Post-Bot.git
   cd Shit-Post-Bot
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure credentials and targets in `config/`.

4. Run the bot:
   ```bash
   python main.py
   ```

---

**Disclaimer:** This project is for educational and research purposes only. Ensure compliance with Facebook’s API Terms of Service and local content laws.
