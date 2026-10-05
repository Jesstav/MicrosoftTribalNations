# GRANTED — Grant Assistant (Tribal Nations)

**Type:** Microsoft Copilot Studio multi-agent solution (importable `.zip`)

GRANTED is an end-to-end **grant discovery, writing, and review** assistant built in Microsoft Copilot Studio for tribal governments and Native-owned enterprises. It is an *orchestrator* agent that routes work through three specialized child agents and always finishes by producing a drafted proposal document.

## What it does

An orchestrator (**GRANTED**) controls a fixed pipeline and never does the child work itself:

1. **Grant Finder** — Identifies and shortlists relevant funding opportunities from official sources (Grants.gov, federal agency sites), returning a verified, source-linked shortlist with eligibility notes and deadlines. Never fabricates eligibility, deadlines, or funding amounts.
2. **Grant Writer** — Once a specific grant is selected, drafts structured proposal content (executive summary, need, approach, workplan, outcomes/metrics, sustainability plan, budget narrative, win themes). Missing facts are flagged as `[FILL-IN REQUIRED]` rather than invented.
3. **Grant Reviewer** — Provides advisory, **non-blocking** feedback on drafts: strengths, required fixes, optional enhancements, and a 0–100 readiness score. Review never blocks document generation.

The flow (**Finder → Writer → Reviewer**) always ends by generating a Word document named `<Grant Title> – Draft Proposal.docx`.

## Capabilities & configuration

- **Web browsing:** enabled (for live source verification)
- **Model hint:** GPT-5 Chat
- **Document generation:** Word (via a WorkIQ Word action)
- **Knowledge sources** wired into the agent:
  - [Grants.gov](https://grants.gov)
  - [Bureau of Indian Affairs — Grants](https://www.bia.gov/topic/grants)
  - [U.S. DOT Build America — Rural and Tribal Grants](https://www.transportation.gov/buildamerica)
  - [Choctaw Nation](https://www.choctawnation.com)
  - A SharePoint **grant-writing library** (templates / boilerplate) — the Writer uses this as its authoritative source for structure and tribal framing

> **Default context (editable):** This export ships with a hard-coded default organization — **Salt River Pima-Maricopa Indian Community (SRPMIC), Phoenix, Arizona** — applied to discovery, drafting, and review unless the user overrides it with a different tribe/location. Change this in the orchestrator and Grant Writer instructions before reuse so proposals reflect the correct organization.

## How to use it

This agent is distributed as a **Copilot Studio solution package**, not as paste-in instructions.

1. Go to [Copilot Studio](https://copilotstudio.microsoft.com) and open your environment.
2. Go to **Solutions → Import solution**.
3. Upload [`solution/GRANTEDAgentTribalNations_1_0_0_1.zip`](./solution/GRANTEDAgentTribalNations_1_0_0_1.zip).
4. After import, open the **GRANTED** agent, reconnect any knowledge sources / connection references for your tenant, update the default tribe/location, and publish.

If you only want to study or reuse the prompt logic (for example in Microsoft Copilot Agent Builder), the plain-text instructions for each agent are in [`instructions/`](./instructions):

| File | Agent |
| --- | --- |
| [`0-orchestrator.txt`](./instructions/0-orchestrator.txt) | GRANTED orchestrator (routing + pipeline) |
| [`1-grant-finder.txt`](./instructions/1-grant-finder.txt) | Grant Finder (discovery) |
| [`2-grant-writer.txt`](./instructions/2-grant-writer.txt) | Grant Writer (drafting) |
| [`3-grant-reviewer.txt`](./instructions/3-grant-reviewer.txt) | Grant Reviewer (QA) |

## Good first prompts

- "Find federal grants for a tribal broadband expansion project in Arizona, up to $2M, deadline in the next 6 months."
- "Draft a proposal for the NTIA Tribal Broadband Connectivity Program for our fiber-to-the-home project."
- "Review this draft executive summary for eligibility alignment and clarity."

## Notes

- Built for the MicrosoftTribalNations gallery as a tribal-focused grants solution.
- Replace knowledge sources, connection references, and the default organization with your own before production use.
