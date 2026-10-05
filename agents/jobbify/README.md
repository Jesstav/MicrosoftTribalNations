# Jobbify — Hiring Intake & Candidate Matching

**Type:** Microsoft Copilot Studio agent (autonomous, email-triggered)

Jobbify is an autonomous recruiting assistant that watches an inbox, detects hiring-related emails, matches open roles against a candidate "hiring bench," and produces an executive-ready candidate comparison — then replies and schedules a follow-up meeting automatically.

> **Note:** This folder ships the agent **instructions only** (no importable `.zip`). The original export embedded a live SharePoint sharing link and internal demo URLs pointing at a resumes folder, so those have been replaced with `[PLACEHOLDER]` values. Wire the agent to **your own** HR SharePoint site, hiring-bench folder, and template before use.

## What it does

When a new email arrives, Jobbify runs this pipeline autonomously (no prompts for permission):

1. **Classify** — Decide whether the email is hiring/job-posting related. If not, stop and do nothing.
2. **Read the role** — Open the job description from the email body, a link, or an attachment, and capture key requirements (technical skills, leadership, cultural/organizational fit, role-specific qualifications).
3. **Match candidates** — Pull resumes from your SharePoint **hiring bench** folder and compare each candidate against the role.
4. **Generate a comparison doc** — Create a Word document from your branded template (preserving header/logo/footer and template styles) titled *"Candidacy Insights & Recommendation"*, with an executive summary and one section per candidate (narrative + bullets for technical ability, leadership, cultural fit, role-specific requirements, overall fit, and a link to each resume).
5. **Reply** — Send a professional, HTML-formatted reply to the original sender confirming review and noting the attached comparison document.
6. **Schedule** — Find a 30-minute slot in the next 7 days (business hours) and send a meeting invite, without waiting for confirmation.

## Capabilities & configuration

- **Model hint:** GPT-5 Chat
- **Trigger:** *When a new email arrives*
- **Actions / connectors used:**
  - Office 365 Users — Get user profile
  - WorkIQ Mail, Calendar, User, and Word (Preview) actions
- **Knowledge sources:** your HR SharePoint site (hiring-bench resumes folder + candidate-comparison template)

## How to use it

This is an autonomous Copilot Studio agent. To rebuild it in your own environment:

1. In [Copilot Studio](https://copilotstudio.microsoft.com), create a new agent and paste the logic from [`instructions.txt`](./instructions.txt) into its instructions.
2. Add your HR SharePoint site as a **knowledge source**, and update the placeholders:
   - `[YOUR HR SHAREPOINT SITE]`
   - `[YOUR HIRING BENCH FOLDER]`
   - `[YOUR CANDIDATE COMPARISON TEMPLATE.docx]`
   - `[ORGANIZATION / LOCATION]` (document subtitle)
3. Add the **Office 365 Users** and **WorkIQ Mail / Calendar / User / Word** actions.
4. Add the **"When a new email arrives"** trigger.
5. Test with a sample hiring email, then publish.

## Caution

- This agent **acts autonomously** — it sends email and creates meetings without asking. Test thoroughly in a safe mailbox before pointing it at a live inbox.
- The hiring bench holds resumes (candidate PII). Keep the SharePoint source permissioned and never expose its sharing links publicly.

## Notes

Built for the MicrosoftTribalNations gallery. Replace all placeholders, knowledge sources, and connection references with your own before production use.
