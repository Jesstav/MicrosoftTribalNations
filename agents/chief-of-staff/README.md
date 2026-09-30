# Chief of Staff (Agent)

A Microsoft 365 Copilot agent that helps you quickly regain control when work piles up. It gives you a clear, structured view of what matters most across your emails, meetings, messages, and tasks — surfacing priorities, risks, and upcoming commitments while ensuring you remain fully in control of every action it recommends.

## Attribution

This agent is adapted from the community **Chief of Staff** sample in the [pnp/copilot-prompts](https://github.com/pnp/copilot-prompts/tree/main/samples/agent-instructions/chief-of-staff-agent) gallery.

- **Original contributor:** Lance Masina — [GitHub](https://github.com/LDMasina) | [LinkedIn](https://linkedin.com/in/lancemasina)
- **License:** MIT (see [`LICENSE`](../../LICENSE))

## Use cases

- **Back from absence** — Retrieve everything that happened while you were out, learn what matters most, and get a clear path back to full operating capacity.
- **Falling behind mid-sprint** — Score your priorities, surface the communications that need attention first, and identify meetings costing more time than they are worth.
- **Weekly planning ritual** — Run the full workflow sequence to lock priorities, protect focus time, and close the week with a clear task brief.
- **Stakeholder relationship health** — Urgency and sentiment detection flags conversations going quiet before they become problems.
- **Connect your sprint board to your wider workload** — Unify Azure DevOps, email, Teams, and Planner into a single view.

## How to build this agent

This is a **Microsoft 365 Copilot declarative agent** — it is built in **Copilot Agent Builder**, not deployed as code.

1. Open **[copilot.microsoft.com](https://copilot.microsoft.com)** (or Copilot in Teams) with an account that has a **Microsoft 365 Copilot license**.
2. Go to **Agents → Create agent → Configure**.
3. **Name:** `Chief of Staff`
4. **Description:** paste the contents of [`description.txt`](./description.txt).
5. **Instructions:** paste the contents of [`instructions.txt`](./instructions.txt) (7,727 characters — within the 8,000 limit).
6. Create the agent and test with: *"I need to get back up to speed."*

## Customization

The instructions are reconfigurable. You may tailor the **default scoring weights**, **tone**, and **persona** to your preference. For the agent to behave like a true Chief of Staff, no other alterations are advised.

## Description

> A precision-oriented productivity recovery agent that acts as the user's personal Chief of Staff within Microsoft 365. It triages workloads, scores and ranks priorities, detects stakeholder urgency, audits meetings, and restructures the user's week into an optimised operating plan. Always recommending, never acting without explicit confirmation.

## Instructions

The full instruction set is in [`instructions.txt`](./instructions.txt).
