# MPB Project Framework (Mind → Paper → Building)

> A tiny, opinionated framework to move from idea → plan → shipped. Includes a Mental Model Library and Starter Macros you can run in ChatGPT or your Cloud agent.

![status](https://img.shields.io/badge/status-active-brightgreen)
![license](https://img.shields.io/badge/license-MIT-blue)

---

## Why MPB?
Most projects stall because people start building without clarity or a plan. MPB enforces a simple order:
- **Mind** → get logic and purpose crystal clear.
- **Paper** → draft a visual plan and test tools (POC).
- **Building** → execute with focus and feedback loops.

This repo packages the framework, mental models, and copy‑paste macros so you can launch in **10 minutes**.

---

## 10‑Minute Quick Start

**Option A — ChatGPT**
1. Create a new custom GPT or chat.
2. Open `prompts/MPB_System_Prompt_MINIMAL.txt` and paste it as the system prompt.
3. Upload:
   - `framework/MPB_Project_Framework.md` (replace with your Notion export)
   - `library/MPB_Mental_Model_Library.md`
   - `library/MPB_Starter_Macros.md`
4. Type: `Run Mind Starter for <your project>`

**Option B — Cloud/Agent Platform**
1. Create a new project/agent.
2. Paste `prompts/MPB_System_Prompt_MINIMAL.txt` into the system prompt field.
3. Upload the three reference files above as the knowledge base.
4. Start with the **Mind Starter** macro.

> Prefer the minimal system prompt; use `prompts/MPB_System_Prompt_FULL.md` if you need stricter behavior.

---

## Repository Structure

```
.
├─ README.md
├─ LICENSE
├─ CHANGELOG.md
├─ CODE_OF_CONDUCT.md
├─ CONTRIBUTING.md
├─ .gitignore
├─ framework/
│  └─ MPB_Project_Framework.md         # Replace with your Notion export
├─ library/
│  ├─ MPB_Mental_Model_Library.md      # Models + Simple Prompts
│  └─ MPB_Starter_Macros.md            # Starter macros for Mind/Paper/Building
├─ prompts/
│  ├─ MPB_System_Prompt_MINIMAL.txt    # Minimal controller prompt
│  └─ MPB_System_Prompt_FULL.md        # Extended controller prompt
├─ examples/
│  ├─ n8n_new_leads_notification.md
│  └─ client_onboarding_automation.md
└─ docs/
   └─ QUICK_REFERENCE.md
```

---

## How to Export from Notion
1. Open your MPB page in Notion → **Export** → **Markdown & CSV**.
2. Rename the exported file to **`MPB_Project_Framework.md`**.
3. Replace the placeholder in `framework/` with your file (keep the same filename).

---

## Examples
- **n8n New Leads Notification** — a minimal MPB automation example (`examples/n8n_new_leads_notification.md`).
- **Client Acquisition & Onboarding** — end-to-end flow for coaches/consultants (`examples/client_onboarding_automation.md`).

---

## Versioning & Releases
We use semantic-ish versions:
- `0.x` — rapid iteration
- `1.0.0` — first stable

Create a GitHub Release when your framework file is ready and tag it (e.g., `v0.1.0`).

---

## Contributing
See [`CONTRIBUTING.md`](CONTRIBUTING.md). Please follow the MPB structure and keep changes concise.

## License
MIT — see [`LICENSE`](LICENSE).

## Maintainers
- Add yourself here (name, website, contact).

---

## FAQ
**Q: Can I use a different license for docs?**  
A: Yes. Keep MIT for simplicity, or split: MIT for code, CC‑BY for docs.

**Q: Do I need the FULL system prompt?**  
A: Start with the minimal prompt; switch to FULL only if you need stricter guardrails.
