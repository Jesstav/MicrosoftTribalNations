# Contributing

Thanks for helping grow this gallery of Microsoft Copilot agents! This guide explains how to add a new agent.

## What this repo is

A curated collection of Microsoft Copilot agents, organized so each is easy to browse and reuse. Two kinds of agents live here:

- **M365 Copilot (Agent Builder)** — declarative agents you build by pasting an *Instructions* block and a *Description* into [Copilot Agent Builder](https://copilot.microsoft.com). These ship with `instructions.txt` + `description.txt`.
- **Copilot Studio (template)** — Microsoft-managed templates you install and configure in [Copilot Studio](https://copilotstudio.microsoft.com). These are documented with a `README.md` only (no paste-in files).

## Folder structure

Each agent gets its own folder under [`agents/`](./agents):

```
agents/
  your-agent-name/
    README.md          # required — what it does + how to build/deploy it
    instructions.txt   # Agent Builder agents only — the paste-ready instructions
    description.txt     # Agent Builder agents only — the paste-ready description
    assets/            # optional — screenshots referenced by the README
```

Use a short, lowercase, hyphenated folder name (e.g., `it-helpdesk`, `budget-grants`).

## How to add an M365 Copilot (Agent Builder) agent

1. Create `agents/<your-agent-name>/`.
2. Add `instructions.txt` — the full instruction set. **Keep it at or under 8,000 characters** (Agent Builder's limit). Verify the count before submitting.
3. Add `description.txt` — a concise one-paragraph description.
4. Add a `README.md` following the pattern of existing agents (summary, why it fits, what it does, build steps, prerequisites, and attribution if adapted).
5. Add a row to the **Agents** table in the top-level [`README.md`](./README.md).

## How to add a Copilot Studio template

1. Create `agents/<your-agent-name>/`.
2. Add a `README.md` covering: what it does, prerequisites, step-by-step deployment, extension opportunities, and limitations. Link to the official Microsoft Learn doc.
3. Add a row to the **Agents** table in the top-level `README.md`.

## Attribution & licensing

- This repo is **MIT-licensed** (see [`LICENSE`](./LICENSE)).
- If your agent is **adapted from a community sample** (e.g., [pnp/copilot-prompts](https://github.com/pnp/copilot-prompts)), credit the **original author and source** in the agent's `README.md`. Only contribute content you have the right to share.
- If your agent is **original**, note that it was built for this gallery.

## Content guidelines

- **This is a public repository.** Never include confidential, internal, or customer data — no real account names, license counts, spend figures, contacts, or other sensitive information. Use `[PLACEHOLDER]` values in examples.
- Keep instructions clear, action-oriented, and free of secrets or credentials.
- Prefer respectful, inclusive language. For agents intended for Tribal Nations audiences, use preferred names and terminology and avoid stereotypes.
- Test your agent in Agent Builder or Copilot Studio before submitting.

## Submitting

1. Fork the repo and create a branch.
2. Add your agent folder and update the top-level `README.md` table.
3. Open a pull request describing the agent, its intended audience, and (if adapted) its source and license.

We'll review for structure, attribution, and the content guidelines above. Thank you for contributing!
