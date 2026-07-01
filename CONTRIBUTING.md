# Contributing to Sovereign AI Starter Pack — Ollama Edition

Thank you for helping improve this pack. This is a **static beginner guide product** — numbered text guides, overview docs, and documentation. Contributions should make local AI setup clearer, safer, and easier for first-time users.

---

## Before You Start

1. Read `README.md` and `00_OVERVIEW.txt`.
2. Review `SECURITY.md` — never submit real passwords, API keys, private prompts, or personal data.
3. Check `LICENSE` — commercial resale of this pack requires written permission from MATTEBLACK STUDIOS.

---

## How to Open Issues

Use GitHub Issues for:

- Broken links or outdated install steps (Ollama, Open WebUI, Docker)
- Confusing wording in numbered guides (`00`–`10`)
- Missing privacy or safety disclaimers
- Model recommendation updates (with sources)
- README / Mermaid diagram mismatches with the text guides

**Good issue titles:**

- `docs: 02_INSTALL_OPENWEBUI Docker command outdated`
- `readme: Super Simple diagram skips optional WebUI path`

**Include in your issue:**

- Which file(s) you read
- Your OS (Mac / Windows / Linux) and rough hardware (RAM)
- What you expected vs. what happened

**Do not open public issues for:**

- Security vulnerabilities with sensitive details → see `SECURITY.md`
- Personal troubleshooting with private data → use the guides locally

---

## How to Submit Improvements

### Pull requests welcome for:

- Documentation clarity (`README.md`, `00`–`10` guides)
- Troubleshooting additions in `07_TROUBLESHOOTING.txt`
- FAQ entries in `08_FAQ.txt`
- Mermaid diagram improvements in `README.md`
- Credits and link fixes in `10_CREDITS.txt`

### Pull request checklist

- [ ] Changes follow existing naming (`NN_TOPIC.txt`, uppercase where used)
- [ ] Install commands match official Ollama and Open WebUI docs
- [ ] `README.md` Quick Start and Workflow Visuals agree with numbered guides
- [ ] No real names, credentials, or private prompts added
- [ ] No `.env`, vault paths, or macOS `._*` junk files included
- [ ] Text files use LF line endings (see `.gitattributes`)

### What we are unlikely to merge without discussion

- Removing core numbered guides
- Adding heavy dependencies (installers, binaries, npm packages)
- Cloud-only workflows that undermine the local-first doctrine
- Content copied from proprietary courses or paid prompt libraries

---

## Pack Structure (Follow This Layout)

```
SOVEREIGN_AI_STARTER_PACK_OLLAMA/
├── README.md                      # Product overview, quick start, Mermaid visuals
├── 00_OVERVIEW.txt                # Big picture
├── 01_INSTALL_OLLAMA.txt          # Ollama install
├── 02_INSTALL_OPENWEBUI.txt       # Optional WebUI
├── 03_MODEL_HORSEPOWER_GUIDE.txt  # RAM / GPU basics
├── 04_MODEL_RECOMMENDATIONS.txt   # Model picks
├── 05_OTHER_POPULAR_TOOLS.txt     # Alternatives
├── 06_HARDWARE_GUIDE.txt          # Hardware guide
├── 07_TROUBLESHOOTING.txt         # Fixes
├── 08_FAQ.txt                     # FAQ
├── 09_SAFETY_AND_PRIVACY.txt      # Safety
├── 10_CREDITS.txt                 # Attribution
├── VERSION.TXT
└── changelog.txt
```

---

## Code of Conduct

This project follows the [Contributor Covenant](CODE_OF_CONDUCT.md). By participating, you agree to uphold a respectful, professional community standard.

---

## Questions

- **Workflow:** `README.md` or `00_OVERVIEW.txt`
- **Install:** `01_INSTALL_OLLAMA.txt`, `02_INSTALL_OPENWEBUI.txt`
- **Problems:** `07_TROUBLESHOOTING.txt`, `08_FAQ.txt`
- **Security:** `SECURITY.md`
- **Attribution:** `10_CREDITS.txt`

---

*Sovereign AI Starter Pack — Ollama Edition — MATTEBLACK STUDIOS*
