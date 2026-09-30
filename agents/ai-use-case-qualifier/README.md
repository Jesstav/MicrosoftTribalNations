# AI Use Case Qualifier (Agent)

A Microsoft 365 Copilot agent that guides partners, consultants, and AI program leads through a **structured qualification conversation** before committing to build an AI solution. It scores the use case across five weighted dimensions, recommends the right Microsoft AI platform, surfaces top risks and success factors, and produces a shareable **qualification report**.

## Attribution

Adapted from the community **The Use Case Qualifier** sample in the [pnp/copilot-prompts](https://github.com/pnp/copilot-prompts/tree/main/samples/agent-instructions/ai-use-case-qualifier) gallery. The methodology is inspired by the Microsoft Jumpstart use-case qualification approach.

- **Original contributor:** Elliot Margot — [GitHub](https://github.com/OwnOptic) (Team Lead Jumpstart – Copilot and Agents, Witivio; Microsoft AI Specialist)
- **License:** MIT (see [`LICENSE`](../../LICENSE))

## Why it fits Tribal Nations

Helps you **qualify AI/Copilot opportunities** across the accounts you support — deciding whether a proposed agent or automation is worth building, which Microsoft platform fits (M365 Copilot, Copilot Studio, Azure AI), and what risks to resolve first. A practical front door before standing up any of the other agents in this gallery.

## What it does

- **Discovery intake** — Captures the scenario, stakeholders, data sources, and desired outcome.
- **Dimension assessment** — Scores across Business Value, Technical Feasibility, Adoption Readiness, Governance, and Delivery Risk (out of 25).
- **Platform fit analysis** — Recommends the best-fit Microsoft AI platform for the use case.
- **Risk & blocker map** — Surfaces the top risks and success factors.
- **Qualification report** — Produces a shareable RED/AMBER/GREEN report with a recommendation and next step.

## How to build this agent

This is a **Microsoft 365 Copilot declarative agent** — built in **Copilot Agent Builder**.

1. Open **[copilot.microsoft.com](https://copilot.microsoft.com)** with a **Microsoft 365 Copilot**–licensed account.
2. Go to **Agents → Create agent → Configure**.
3. **Name:** `AI Use Case Qualifier`
4. **Description:** paste the contents of [`description.txt`](./description.txt).
5. **Instructions:** paste the contents of [`instructions.txt`](./instructions.txt) (7,088 characters — within the 8,000 limit).
6. Create the agent and test with a use case, e.g. *"I want to qualify an AI contract-review idea."*

## Prerequisites

- A **Microsoft 365 Copilot** license.

## Instructions

The full instruction set is in [`instructions.txt`](./instructions.txt).
