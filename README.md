# Sebastián Espindola

Customer-facing operations and AI solutions professional building practical automation systems. I translate messy operational workflows into guided, reliable experiences for customers and internal teams.

- 🌎 Based in Colombia · fluent English (C2)
- 🎯 Focus: API integrations, workflow automation, data management, and customer-facing technical solutions
- 📫 Reach me at [sebastian.espindola.h@gmail.com](mailto:sebastian.espindola.h@gmail.com)

## Selected automation projects

### Declara Fácil — Guided tax-document intake bot

**Operational pain relieved:** Preparing an income-tax case often begins with scattered documents, uncertainty about which supports apply, incomplete submissions, and repeated manual follow-up. That creates delays for both the client and the tax-preparation team.

**What it does:** A Telegram bot guides each client through a short decision flow, requests only the documents relevant to their situation, tracks progress, receives files, and makes it possible to request human help when the case needs it.

**How it works:**

```text
Client on Telegram
  → guided eligibility and document questions
  → structured case and document-status records
  → secure file handoff to the team workflow
  → spreadsheet-based operational visibility
  → human escalation when needed
```

**Implementation highlights:** Cloudflare Worker webhook, Telegram Bot API, Cloudflare D1 for structured client and workflow state, conditional document checklist, duplicate-safe status updates, Google Drive/Sheets integration through OAuth, and a human-in-the-loop escalation path. The design explicitly avoids requesting passwords, verification codes, or electronic signatures through chat.

**Skills demonstrated:** API integration, webhook handling, relational data modeling, OAuth-based integrations, operational workflow design, data validation, and customer communication.

---

### Secretaria Casanova — Conversational quotation and PDF bot

**Operational pain relieved:** Creating quotes for events and production services can be repetitive: staff must collect recipient details, line items, quantities, prices, tax choices, calculate totals, format a document, and send it back. Manual handoffs introduce delays and calculation or formatting mistakes.

**What it does:** A Telegram bot walks a user through the quote step by step, supports multiple line items, calculates subtotal and optional VAT, lets the user review or correct key fields, and returns a polished PDF quotation in the same conversation.

**How it works:**

```text
Client on Telegram
  → guided quote form in chat
  → saved session and line items
  → subtotal / VAT / total calculation
  → PDF generation
  → quotation delivered back in Telegram
```

**Implementation highlights:** Cloudflare Worker webhook, Telegram Bot API, Cloudflare D1 session state, input parsing for prices and quantities, interactive Telegram buttons, generated PDF output, calculation logic, and a review-and-correction step before finalization.

**Skills demonstrated:** event-driven workflow design, stateful conversations, input validation, data transformation, document generation, API integration, and user-centered automation.

## What I build

I enjoy solving the gap between a business process and the systems that support it:

- Map business rules into clear data flows and system behavior.
- Connect services through APIs and webhooks.
- Design reliable intake, tracking, escalation, and reporting workflows.
- Explain technical decisions clearly to nontechnical users.
- Keep security and privacy in scope by using managed secrets and avoiding sensitive data in code or documentation.

<!--
This is a special repository: its README appears on the GitHub profile.
-->
