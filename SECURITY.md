# Security Policy

**Sovereign AI Starter Pack — Ollama Edition — MATTEBLACK STUDIOS**

This pack is a local-first AI guide product. It ships static documentation only. It does not run servers, collect telemetry, or store user data.

---

## Reporting a Vulnerability

If you discover a security issue in this repository (for example: accidental inclusion of secrets, credentials, personal data, or instructions that could cause unsafe data handling), please report it responsibly.

**Preferred contact:** [https://matteblackstudios.com](https://matteblackstudios.com)

When reporting, include:

- A clear description of the issue
- The file path(s) affected
- Steps to reproduce (if applicable)
- Your recommended fix (if you have one)

**Please do not** open a public GitHub issue for sensitive security reports. We will acknowledge receipt and work to resolve confirmed issues promptly.

---

## Privacy Expectations

This pack is designed with a **privacy-first, local-first** doctrine:

| What this pack does | What this pack does **not** do |
|---|---|
| Teaches local Ollama and Open WebUI setup | Store, log, or transmit your chat content |
| Documents privacy best practices | Control how third-party tools handle your data |
| Recommends local-only habits | Guarantee anonymity if you enable cloud features elsewhere |

**Your responsibility:**

- Keep Ollama and Open WebUI on localhost unless you intentionally expose them
- Do not paste passwords, bank details, or medical records into any AI
- Review model licenses and provider terms for any optional cloud add-ons
- Delete chat history and models when sharing a computer

See `09_SAFETY_AND_PRIVACY.txt` and `README.md` for guidance.

---

## Safe Usage Guidelines

1. **Verify important facts** — Local models can hallucinate. Confirm medical, legal, and financial information independently.
2. **Bind services locally** — Open WebUI should run on `localhost` for personal use. Do not expose Ollama to the public internet without hardening.
3. **Use strong local accounts** — If Open WebUI requires a login, use a strong password on shared machines.
4. **Update regularly** — Keep Ollama, Open WebUI, Docker, and models patched.
5. **Anonymize when testing** — Replace real names and identifiers when experimenting or submitting example issues.
6. **Delete when done** — Remove models and chat exports you no longer need on shared devices.

This pack is **not** legal, medical, or financial advice.

---

## Data This Pack Must Never Contain

Contributors and users must **not** commit or submit the following into this repository or into issues/PRs:

### No personally identifiable information (PII)

- Real names, addresses, phone numbers, or email addresses
- Private chat logs or prompts containing sensitive content
- Employer or client confidential information

### No secrets

- API keys, tokens, passwords, or `.env` files
- Docker registry credentials or SSH private keys

### No copyrighted third-party content

- Do not copy proprietary install guides, paid courses, or licensed prompt libraries into this repo
- Link to official Ollama and Open WebUI documentation instead

If you are unsure whether content is safe to contribute, **do not include it** — open a general question issue instead.

---

## Scope

This security policy covers:

- The static files in this repository
- Documentation accuracy and safe-use guidance
- Accidental inclusion of secrets or personal data in commits

This policy does **not** cover:

- Security of Ollama, Open WebUI, Docker, or model weights
- Your local device, network, firewall, or VM configuration
- How you expose or share local AI services on your LAN or WAN

---

*Sovereign AI Starter Pack — Ollama Edition v1.1 — MATTEBLACK STUDIOS*
*Local-first. Privacy-first. Studio-grade.*
