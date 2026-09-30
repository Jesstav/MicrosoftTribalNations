# Sustainability Insights (Agent)

A Microsoft **Copilot Studio** agent template that helps you uncover insights and data about your company's sustainability goals and progress. It can compare your efforts year over year and against other organizations, and answer general sustainability questions — all grounded in the knowledge sources you provide.

> **Note:** Like [IT Helpdesk](../it-helpdesk) and [Website Q&A](../website-qanda), this is a **Copilot Studio managed template**. It ships with prebuilt topics and messages and is configured in Copilot Studio — there is no instructions block to paste. This folder documents how to deploy it.

## Source

- **Publisher:** Microsoft
- **Official docs:** [Sustainability Insights template — Microsoft Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/template-sustainability-insights)

## What it does

- Answers questions about your organization's sustainability progress and efforts (e.g., *"What is our total greenhouse gas emissions?"*, *"What are our scope 1 emissions?"*).
- Compares **year-over-year** results (e.g., *"What were our greenhouse gas emissions in 2023 compared to 2022?"*).
- Benchmarks against **other organizations** (e.g., *"How do our scope 1 emissions compare to [other organization]?"*).

Ships with prebuilt topics and messages to jump-start building your own sustainability agent.

## Use cases

- **Sustainability reporting** — Surface KPIs from ESG and corporate-responsibility reports on demand.
- **Year-over-year analysis** — Track progress across multiple reporting periods.
- **Peer benchmarking** — Compare your metrics with an industry peer or supplier's public data.

## Prerequisites

- A **Copilot Studio** account/license.
- A **source of sustainability information** (internal documents, websites, ESG/CSR reports).
- *Optional:* Links to other organizations' public sustainability sources for comparison.

## How to deploy

1. On the **Agents** page in [Copilot Studio](https://copilotstudio.microsoft.com), under **Start with an agent template**, select **Sustainability Insights**.
2. Update the agent **name, description, and instructions** (and optionally icon/language), then select **Create**.
3. Replace the default **knowledge sources** with links to your organization's sustainability sources (reports across multiple years, CSR portals, etc.).
4. Fine-tune by adding/updating **required topics** and prebuilt messages.
5. Select **Test** and validate responses against your knowledge sources.
6. Select **Publish** to release the agent.

### Benchmarking with other organizations

To compare across companies, set the `OrganizationName` (your company) and `OrganizationToCompare` variables in the *Conversation Start* topic, and configure knowledge sources for both. The agent retrieves data for each, then compares the datasets. For best results, ensure both sources contain **overlapping, comparable data points**.

## Tips

- If data won't extract from tables in PDF reports, use the **Excel Power Query** plugin to pull the tables, save them as **CSV**, and upload the CSVs as additional knowledge sources.
- Sustainability KPIs vary by reporting period — specify the period (e.g., 2022 vs. 2023). You can build a custom topic with Trigger and Question nodes plus a Power Fx formula to extract KPI values for a chosen period.

## Limitations

Managed agents and agent templates are currently **English only** and intended for **internal use** within your organization. Comparison quality depends entirely on the data sources provided. AI-generated content can contain mistakes — review responses for accuracy. See the [Supplemental Terms](https://go.microsoft.com/fwlink/?linkid=2189520).
