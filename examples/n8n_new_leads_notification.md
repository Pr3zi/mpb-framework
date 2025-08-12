# Example: n8n Automated New Leads Notification (with Mental Models)

## 🧠 Mind
- **Goal:** Instantly notify sales when a new lead hits the CRM.
- **Logic:** Trigger (new CRM record) → Filter (qualified) → Format → Notify (Slack/email) → Backup (Sheets).
- **Models:** First Principles, Inversion, 80/20.

## ✍️ Paper
- **Diagram:** Trigger → Filter → Formatter → Notification → Backup.
- **Tools:** n8n, Slack, Gmail/Outlook, Google Sheets, CRM (HubSpot/Pipedrive).
- **POC:** Send a sample lead; verify message formatting.
- **Models:** Bottleneck, Critical Path, Red Team.

## 🛠️ Building
- **Nodes:** CRM Trigger, IF Filter, Set, Slack, Google Sheets.
- **Add:** Error handling and logging.
- **Models:** Feedback Loops, Checklist Manifesto, Premortem.

**Exit Criteria:** Right info reaches the right person instantly; no manual CRM checks.
