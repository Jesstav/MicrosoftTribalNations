# MicrosoftTribalNations — Copilot Agent Gallery

A collection of Microsoft 365 Copilot agent instructions, packaged so they are easy to browse and paste into **Copilot Agent Builder**.

Each agent lives in its own folder under [`agents/`](./agents) and includes:

- `README.md` — what the agent does and how to build it
- `instructions.txt` — the paste-ready instructions block (Agent Builder has an 8,000-character limit)
- `description.txt` — the paste-ready description
- `assets/` — optional screenshots

## Agents

| Agent | Type | Description |
|-------|------|-------------|
| [Chief of Staff](./agents/chief-of-staff) | M365 Copilot (Agent Builder) | Triages your workload, scores priorities, detects stakeholder urgency, audits meetings, and rebuilds your week — always recommending, never acting without confirmation. |
| [Promptly](./agents/promptly) | M365 Copilot (Agent Builder) | Helps you craft effective AI prompts with warm, step-by-step coaching and side-by-side refinements. |
| [Customer Comments](./agents/customer-comments) | M365 Copilot (Agent Builder) | Reviews customer/member feedback and drafts professional, empathetic responses grounded in your complaint-handling guidelines. |
| [Finance — Budget & Grants Assistant](./agents/finance) | M365 Copilot (Agent Builder) | Answers tribal budget and federal-funding questions, tracks grant balances and reporting deadlines, and drafts briefings — always source-cited. |
| [Specific Research](./agents/specific-research) | M365 Copilot (Agent Builder) | Finds and formats recent news articles on a topic you specify — useful for policy and regulatory monitoring. |
| [Communications Assistant](./agents/communications) | M365 Copilot (Agent Builder) | Drafts clear, respectful comms — emails, letters, announcements, newsletters, social posts, and press releases — always for your review. |
| [IT Helpdesk](./agents/it-helpdesk) | Copilot Studio (template) | Resolves helpdesk issues from your ServiceNow knowledge base, escalates via ServiceNow tickets, and lets employees track their cases. |
| [Website Q&A](./agents/website-qanda) | Copilot Studio (template) | Answers customer questions using your website's content, with generative AI formulating contextual responses. |
| [Sustainability Insights](./agents/sustainability-insights) | Copilot Studio (template) | Surfaces sustainability KPIs and progress from your reports, compares year-over-year, and benchmarks against other organizations. |
| [Safe Travels](./agents/safe-travels) | Copilot Studio (template) | Gives employees travel documentation, health/safety, and emergency guidance through a conversational interface. |
| [Benefits](./agents/benefits) | Copilot Studio (template) | Helps employees/members understand and compare their benefits, answering tailored questions in seconds. |

## How to use an agent

**Agent Builder agents** (Chief of Staff, Promptly):

1. Open **[copilot.microsoft.com](https://copilot.microsoft.com)** with a Microsoft 365 Copilot–licensed account.
2. **Agents → Create agent → Configure.**
3. Paste the agent's `description.txt` into **Description** and `instructions.txt` into **Instructions**.
4. Create and test.

**Copilot Studio templates** (IT Helpdesk): follow the deployment steps in the agent's own README — these are installed and configured in [Copilot Studio](https://copilotstudio.microsoft.com), not pasted in.

## Attribution & license

Agents adapted from community samples retain their original attribution in each agent's `README.md`. This repository is released under the [MIT License](./LICENSE).