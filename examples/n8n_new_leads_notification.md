## **N8N Example: Automated New Leads Notification System (with Mental Models)**

---

### **🧠 Stage 1: Mind**

**Description:**

At this stage, the focus is on defining the *why* and *what* of the automation before touching any tools. The aim is to gain complete logical clarity on how the new leads notification system will improve sales efficiency.

**Key Actions:**

- Define the exact trigger: e.g., new record in CRM (Pipedrive, HubSpot, Airtable).
- Decide the notification channel: Slack, Discord, or email.
- Identify essential lead information for the notification.
- Clarify recipients and expected reaction time.

**Benefits:**

- Eliminates unnecessary workflow complexity.
- Aligns automation purpose with sales goals.
- Ensures you only collect and send the most valuable data.

**Practical Tips:**

- Start with the simplest possible flow: Trigger → Notification.
- Limit notifications to qualified leads to avoid noise.
- Document your logic before designing the workflow in N8N.

**Outcome:**

A clear mental map of how the notification system will work, who it will serve, and what success looks like.

**Mental Models Applied:**

- **First Principles Thinking** – Reduce the workflow to its bare essentials: trigger, notify, store.
- **Inversion** – List top 3 reasons the system could fail and prevent them early.
- **Pareto Principle (80/20)** – Identify the 20% of lead data that gives 80% of value to sales.

---

### **✍️ Stage 2: Paper**

**Description:**

This is where the concept turns into a visual and logical plan. The workflow is mapped, risks are spotted, and the setup sequence is defined.

**Key Actions:**

1. **Trigger:** New lead created in CRM.
2. **Filter:** Send notifications only for specific lead criteria (location, budget, etc.).
3. **Formatter:** Standardize and clean lead info for clear display.
4. **Notification:** Send formatted info to Slack/email.
5. **Backup:** Save lead data in Google Sheets.

**Benefits:**

- Ensures workflow steps are clear before building.
- Reduces risk of misconfigurations.
- Identifies resource or tool limitations early.

**Practical Tips:**

- Build the workflow diagram before touching N8N.
- Test logic with one sample lead before scaling.
- Keep a note of API rate limits and required field mappings.

**Outcome:**

A complete process map ready for implementation in N8N.

**Mental Models Applied:**

- **Bottleneck Principle** – Spot primary risks: API limits, mapping errors.
- **Critical Path Method** – Arrange workflow steps in the optimal order.
- **Red Team Thinking** – Challenge the plan to find weak spots before building.

---

### **🔧 Stage 3: Building**

**Description:**

Here, the plan becomes a live automation in N8N, tested and prepared for real-world usage.

**Key Actions:**

- Add **Trigger node** for CRM integration.
- Configure **Filter node** (IF conditions).
- Use **Set node** to map and clean fields.
- Add **Slack node** for sending messages.
- Add **Google Sheets node** to append backup data.
- Implement error handling and logging.

**Benefits:**

- Automation works end-to-end without manual checks.
- Sales team gets immediate, accurate notifications.
- Reduces time-to-response and increases conversion rate.

**Practical Tips:**

- Test using real leads before going live.
- Simulate errors to confirm recovery logic works.
- Keep a versioned copy of the workflow for rollback.

**Outcome:**

A fully functioning, resilient lead notification system running in N8N.

**Mental Models Applied:**

- **Feedback Loops** – Use test notifications to verify success continuously.
- **Checklist Manifesto** – Confirm all nodes are properly configured before publishing.
- **Premortem Analysis** – Anticipate failure scenarios and build in prevention.

---

**✅ Quick Exit Criteria:**

- Sales team receives correct lead info instantly, every time.
- No manual CRM checks are needed.
