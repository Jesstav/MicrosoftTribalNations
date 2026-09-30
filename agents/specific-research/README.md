# Specific Research (News) Agent

A Microsoft 365 Copilot agent that finds and shares recent, relevant news articles on topics you specify. Each result is less than a month old and includes the title, publication date, author, source, a brief description, and a link — formatted for easy reading.

## Attribution

Adapted from the community **Specific News research Agent** sample in the [pnp/copilot-prompts](https://github.com/pnp/copilot-prompts/tree/main/samples/agent-instructions/specific-research-agent) gallery.

- **Original contributor:** Robin Le Bourhis — [GitHub](https://github.com/RobinLB-devo)
- **License:** MIT (see [`LICENSE`](../../LICENSE))

## Why it fits Tribal Nations

Handy for **policy and regulatory monitoring** — tracking news on tribal affairs, BIA/IHS updates, federal funding, gaming regulation, or specific accounts and initiatives.

## What it does

- Returns **5 recent articles** (each < 1 month old) on a topic you specify.
- For each: title, publication date, author (if listed), source site, a brief description, and a "Read the article" link, with an illustrative emoji.
- Uses a friendly, well-spaced reply format.

## How to build this agent

This is a **Microsoft 365 Copilot declarative agent** — built in **Copilot Agent Builder**.

1. Open **[copilot.microsoft.com](https://copilot.microsoft.com)** with a **Microsoft 365 Copilot**–licensed account.
2. Go to **Agents → Create agent → Configure**.
3. **Name:** `Specific Research`
4. **Description:** paste the contents of [`description.txt`](./description.txt).
5. **Instructions:** paste the contents of [`instructions.txt`](./instructions.txt) — replace the `[Specific Themes]` / `[Specific topic]` placeholders with your subject and add your first name to the greeting.
6. Enable **web search** so it can retrieve current articles, then create and test.

## Prerequisites

- A **Microsoft 365 Copilot** license (Copilot Chat or Microsoft 365 Copilot).

## Instructions

The full instruction set is in [`instructions.txt`](./instructions.txt).
