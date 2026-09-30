# Budget & Grants Assistant (Finance)

A Microsoft 365 Copilot agent that acts as a plain-language **budget and grants assistant** for a Tribal Nation's government, enterprises, and program staff. It answers budget and federal-funding questions, tracks grant balances and reporting deadlines, and drafts briefings — always citing its sources, never inventing figures, and deferring legal, tax, and audit judgments to the appropriate officer.

> **Custom agent:** Built for this gallery (not adapted from a community sample). It is grounded entirely in the knowledge sources you provide — connect your own budgets, award notices, and grant agreements before relying on it.

## Why it fits Tribal Nations

Purpose-built for **tribal budgets, federal awards, and grant compliance** — funding from IHS, BIA, HUD, Treasury, and similar agencies — including period-of-performance tracking, match/cost-share, federal financial reporting (e.g., SF-425), and Uniform Guidance (2 CFR 200) considerations.

## What it does

- **Budget lookup** — Budgeted vs. actuals vs. remaining by fund/department/program, with the source document and fiscal year cited, and variance explained in plain language.
- **Grant tracker** — Award dates, totals, amounts drawn, match requirements, and reporting deadlines (flagging anything due within 30 days).
- **Compliance support** — Explains reporting obligations and required data points, and provides checklists — without completing or certifying federal forms.
- **Plain-language Q&A & briefings** — Answers staff/leadership questions and drafts Council or program briefings for your review.

## How to build this agent

This is a **Microsoft 365 Copilot declarative agent** — built in **Copilot Agent Builder**.

1. Open **[copilot.microsoft.com](https://copilot.microsoft.com)** with a **Microsoft 365 Copilot**–licensed account.
2. Go to **Agents → Create agent → Configure**.
3. **Name:** `Budget & Grants Assistant`
4. **Description:** paste the contents of [`description.txt`](./description.txt).
5. **Instructions:** paste the contents of [`instructions.txt`](./instructions.txt).
6. Add your budgets, award notices, grant agreements, and finance policies as **knowledge sources**, then create and test.

## Prerequisites

- A **Microsoft 365 Copilot** license.
- Your organization's financial documents added as knowledge sources.

## Guardrails

Cites the document and fiscal year behind every figure; never states a number that isn't in the knowledge sources; never gives legal, tax, or audit opinions or certifies federal forms; flags figures that look over budget, past due, or inconsistent and recommends reconciliation.

## Instructions

The full instruction set is in [`instructions.txt`](./instructions.txt).
