# Sovereign AI Starter Pack — Ollama Edition

**By MATTEBLACK STUDIOS**

> **Disclaimer:** This pack teaches you to run open-source AI models on your own hardware. Model outputs may be inaccurate. Always verify important information. This pack is not legal, medical, or financial advice. You are responsible for how you use AI tools and for complying with model licenses and local laws.

---

## What This Pack Does

The Sovereign AI Starter Pack — Ollama Edition is a beginner-friendly, text-only guide to running AI **locally** on your own computer. Install Ollama, optionally add Open WebUI for a browser chat UI, download a model, and start prompting — with no cloud account, no subscription, and no data leaving your machine by default.

**You do not need to be a developer.** If you can install an app and copy a command into Terminal or PowerShell, you can run local AI.

---

## Who This Is For

- Beginners who want **private, local AI** without cloud lock-in
- Privacy-conscious users who want prompts to stay on their hardware
- Students, writers, and hobbyists exploring open-source models
- Anyone curious about **sovereign compute** before trying advanced workflow packs
- Mac, Windows, and Linux users with modest hardware (8 GB RAM minimum)

If you want ChatGPT-style chat **on your machine**, this pack is your starting line.

---

## Requirements

| Requirement | Minimum | Recommended |
|---|---|---|
| **OS** | macOS 12+, Windows 10/11, or Linux | Latest stable release |
| **RAM** | 8 GB | 16 GB+ |
| **Disk** | 10 GB free | 20 GB+ for multiple models |
| **GPU** | Optional | Apple Silicon or NVIDIA for speed |
| **Internet** | Required for install and first model download | Stable connection for large pulls |
| **Ollama** | [ollama.com/download](https://ollama.com/download) | Latest version |
| **Open WebUI** | Optional — Docker Desktop or pip | Docker method in `02_INSTALL_OPENWEBUI.txt` |

---

## Quick Start

### 1. Install Ollama

Download from **[ollama.com/download](https://ollama.com/download)**, then verify:

```bash
ollama --version
```

Full walkthrough: `01_INSTALL_OLLAMA.txt`

### 2. (Optional) Install Open WebUI

Adds a browser chat UI at `http://localhost:3000`. Ollama works fine from the terminal alone.

Full walkthrough: `02_INSTALL_OPENWEBUI.txt`

### 3. Download and run your first model

```bash
ollama run llama3.2
```

The first run downloads the model. Type a message and press **Enter**. Exit with **Ctrl + C**.

### 4. Read the guides in order

Start with `00_OVERVIEW.txt`, then follow the numbered files. Use `07_TROUBLESHOOTING.txt` if something breaks.

---

## Folder Structure

```
SOVEREIGN_AI_STARTER_PACK_OLLAMA/
├── README.md                      # Product overview (this file)
├── 00_OVERVIEW.txt                # Big picture — start here after README
├── 01_INSTALL_OLLAMA.txt          # Install Ollama (Mac / Windows / Linux)
├── 02_INSTALL_OPENWEBUI.txt       # Optional browser UI (Docker + pip)
├── 03_MODEL_HORSEPOWER_GUIDE.txt  # RAM, GPU, and model size basics
├── 04_MODEL_RECOMMENDATIONS.txt   # Which model to pick first
├── 05_OTHER_POPULAR_TOOLS.txt     # GPT4All, LM Studio, Jan, Kobold
├── 06_HARDWARE_GUIDE.txt          # Hardware limits and upgrades
├── 07_TROUBLESHOOTING.txt         # Problem → fix reference
├── 08_FAQ.txt                     # Quick answers
├── 09_SAFETY_AND_PRIVACY.txt      # Privacy and responsible use
├── 10_CREDITS.txt                 # Tool attribution and links
├── VERSION.TXT                    # Current pack version
├── changelog.txt                  # Release history
├── LICENSE                        # MIT (Modified for Sovereign AI Workflow Packs)
├── CONTRIBUTING.md                # How to open issues and submit improvements
├── SECURITY.md                    # Security reporting and safe-use policy
└── CODE_OF_CONDUCT.md             # Community standards
```

---

## Workflow Visuals

Read left to right. Each box maps to a numbered guide in this pack.

### Full Ollama Starter Workflow

```mermaid
flowchart LR
subgraph INSTALL["INSTALL"]
A["Install Ollama<br/>01_INSTALL_OLLAMA.txt<br/>Mac, Windows, or Linux"]
B["Install Open WebUI<br/>02_INSTALL_OPENWEBUI.txt<br/>(optional)"]
end
subgraph RUN["RUN SERVICES"]
C["Start Ollama<br/>ollama serve<br/>or open Ollama app"]
D["Start Open WebUI<br/>Docker or pip<br/>localhost:3000"]
end
subgraph MODEL["FIRST MODEL"]
E["Download Model<br/>ollama pull llama3.2<br/>04_MODEL_RECOMMENDATIONS.txt"]
F["Run First Prompt<br/>ollama run llama3.2<br/>or chat in Open WebUI"]
end
subgraph GROW["GO DEEPER"]
G["Tune for Hardware<br/>03_MODEL_HORSEPOWER_GUIDE.txt<br/>06_HARDWARE_GUIDE.txt"]
H["Add Memory Pack<br/>Optional sovereign context<br/>MATTEBLACK STUDIOS packs"]
I["Add Workflow Pack<br/>Prompts and templates<br/>MATTEBLACK STUDIOS packs"]
J["Export Results<br/>Copy chat, save notes<br/>09_SAFETY_AND_PRIVACY.txt"]
end
A --> B
B --> C
A --> C
C --> D
C --> E
D --> F
E --> F
F --> G
G --> H
H --> I
I --> J
style A fill:#e3f2fd,stroke:#1976d2
style B fill:#fff8e1,stroke:#f9a825
style E fill:#e8f5e9,stroke:#388e3c
style F fill:#f3e5f5,stroke:#7b1fa2
style J fill:#e8f5e9,stroke:#2e7d32
```

| Step | What you do | File |
|---|---|---|
| Install Ollama | Download and verify the CLI | `01_INSTALL_OLLAMA.txt` |
| Open WebUI | Optional browser chat | `02_INSTALL_OPENWEBUI.txt` |
| Start services | Run Ollama (and WebUI if used) | Guides above |
| Pick a model | Match model to your RAM | `04_MODEL_RECOMMENDATIONS.txt` |
| First prompt | Terminal or WebUI chat | `00_OVERVIEW.txt` |
| Stay private | Local-only habits | `09_SAFETY_AND_PRIVACY.txt` |
| Fix issues | Common errors | `07_TROUBLESHOOTING.txt` |

**Memory and workflow packs** are optional next steps in the MATTEBLACK STUDIOS sovereign AI line — use them once Ollama is running reliably.

### Super Simple (6 Steps)

Six steps. No jargon. If you only remember one picture, remember this one.

```mermaid
flowchart TD
S1["STEP 1: INSTALL OLLAMA<br/><br/>Download from ollama.com<br/>Verify with ollama --version<br/><br/>01_INSTALL_OLLAMA.txt"]
S2["STEP 2: INSTALL OPEN WEBUI<br/><br/>Optional browser chat UI<br/>Skip if terminal is fine<br/><br/>02_INSTALL_OPENWEBUI.txt"]
S3["STEP 3: RUN OLLAMA<br/><br/>Open the app or run<br/>ollama serve<br/><br/>01_INSTALL_OLLAMA.txt"]
S4["STEP 4: RUN WEBUI<br/><br/>Open http://localhost:3000<br/>Create local account<br/><br/>02_INSTALL_OPENWEBUI.txt"]
S5["STEP 5: DOWNLOAD MODEL<br/><br/>ollama pull llama3.2<br/>Wait for download<br/><br/>04_MODEL_RECOMMENDATIONS.txt"]
S6["STEP 6: RUN PROMPT<br/><br/>ollama run llama3.2<br/>Type and press Enter<br/><br/>00_OVERVIEW.txt"]
S1 --> S2 --> S3 --> S4 --> S5 --> S6
style S1 fill:#e1f5fe,stroke:#0288d1,stroke-width:2px
style S2 fill:#fff9c4,stroke:#f9a825,stroke-width:2px
style S3 fill:#e8eaf6,stroke:#3949ab,stroke-width:2px
style S4 fill:#f3e5f5,stroke:#8e24aa,stroke-width:2px
style S5 fill:#fff3e0,stroke:#fb8c00,stroke-width:2px
style S6 fill:#e8f5e9,stroke:#43a047,stroke-width:3px
```

**The whole thing in one sentence:** Install Ollama, optionally add WebUI, run both, pull a model, chat — done.

---

## Useful Commands

```bash
ollama list              # show installed models
ollama pull <name>       # download a model
ollama run <name>        # chat with a model
ollama rm <name>         # delete a model
```

### Recommended starter models

| Situation | Command |
|-----------|---------|
| Best first pick | `ollama run llama3.2` |
| 8 GB RAM or want speed | `ollama run mistral` |
| Low-RAM laptop | `ollama run phi3` |
| Coding and logic | `ollama run qwen2.5` |
| Writing and conversation | `ollama run gemma2` |

Too slow or crashing? Try `ollama run phi3` or `ollama run llama3.2:1b`.

---

## Documentation Order

| Step | File | When to open |
|------|------|--------------|
| 1 | `00_OVERVIEW.txt` | Big picture before installing |
| 2 | `01_INSTALL_OLLAMA.txt` | Installing Ollama |
| 3 | `04_MODEL_RECOMMENDATIONS.txt` | Picking or switching models |
| 4 | `02_INSTALL_OPENWEBUI.txt` | Browser chat UI (optional) |
| 5 | `03_MODEL_HORSEPOWER_GUIDE.txt` | RAM, GPU, and model size |
| 6 | `06_HARDWARE_GUIDE.txt` | Hardware limits and upgrades |
| 7 | `09_SAFETY_AND_PRIVACY.txt` | Privacy and responsible use |
| 8 | `05_OTHER_POPULAR_TOOLS.txt` | GPT4All, LM Studio, Jan, and more |
| 9 | `08_FAQ.txt` | Quick questions |
| 10 | `07_TROUBLESHOOTING.txt` | Something is not working |
| 11 | `10_CREDITS.txt` | Tool attribution and links |

Version info: `VERSION.TXT` and `changelog.txt`

---

## Privacy and Sovereign Compute

This pack is built on **local-first, privacy-first** principles:

- **Your prompts stay on your machine** when you use Ollama locally
- **No account required** for basic Ollama use
- **You control models** — install, switch, and delete anytime
- **Offline capable** after models are downloaded

Read `09_SAFETY_AND_PRIVACY.txt` before pasting sensitive data into any AI tool.

---

## Troubleshooting

| Problem | What to try |
|---------|-------------|
| `ollama` command not found | Close terminal, reopen, restart computer |
| Model won't download | Check internet and disk space; run `ollama pull llama3.2` |
| Out of memory | Use `ollama run phi3`; close other apps |
| Very slow replies | Use a smaller model; plug in your laptop |
| Open WebUI won't open | See `02_INSTALL_OPENWEBUI.txt` and `07_TROUBLESHOOTING.txt` |

Full fix list: `07_TROUBLESHOOTING.txt`

---

## Get the Full Pack

**Gumroad:** [https://gumroad.com/l/sovereign-ai-starter-pack-ollama](https://gumroad.com/l/sovereign-ai-starter-pack-ollama) *(placeholder — update with your live product URL)*

The GitHub repo mirrors the product documentation. The Gumroad download is the customer distribution bundle.

---

## Community and Security

- **Report a security issue** → `SECURITY.md` (do not post sensitive reports in public issues)
- **Contribute improvements** → `CONTRIBUTING.md`
- **Community standards** → `CODE_OF_CONDUCT.md`

---

## License

This pack is released under the [MIT License (Modified for Sovereign AI Workflow Packs)](LICENSE). Commercial resale requires written permission from MATTEBLACK STUDIOS.

---

## Support

- **Website:** [matteblackstudios.netlify.app](https://matteblackstudios.netlify.app)
- **Email:** matteblackstudios1@gmail.com

---

*Sovereign AI Starter Pack — Ollama Edition — MATTEBLACK STUDIOS*
*Local-first. Privacy-first. Studio-grade.*
