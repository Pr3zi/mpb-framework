# Example: Client Acquisition & Onboarding Automation (Coaches & Consultants)

## 🧠 Mind
- **Goal:** Fully automate from inquiry → scheduled call → onboarding materials.
- **Logic:** Form submit → Auto-schedule → CRM entry → Pre-call email → Guide → Reminder.
- **Models:** First Principles, Inversion, 80/20.

## ✍️ Paper
- **Diagram:** Trigger (form) → Scheduler → CRM → Email → Guide → Reminder → Logs.
- **Tools:** Calendly/Book Like A Boss, n8n, Notion/HubSpot, Gmail/Outlook, Google Sheets.
- **POC:** Test with 1 fake lead; confirm email deliverability.
- **Models:** Bottleneck, Critical Path, Red Team.

## 🛠️ Building
- **Nodes:** Webhook, CRM create, Email send, File/link share, Reminder, Logging.
- **Add:** Duplicate prevention, error handling.
- **Models:** Feedback Loops, Checklist Manifesto, Premortem.

**Exit Criteria:** New leads auto-added to CRM; onboarding mails sent; zero manual work.
