# IT Helpdesk (Agent)

A Microsoft **Copilot Studio** agent template that uses your organization's knowledge base to resolve helpdesk issues, escalate to **ServiceNow** when needed, and let employees track their tickets.

> **Note:** Unlike the [Chief of Staff](../chief-of-staff) agent (a declarative agent you build by pasting instructions into Agent Builder), IT Helpdesk is a **Copilot Studio managed template**. You install it from Copilot Studio and configure it — there is no instructions block to copy. This folder documents how to deploy it.

## Source

- **Publisher:** Microsoft
- **Official docs:** [IT Helpdesk template — Microsoft Copilot Studio](https://learn.microsoft.com/en-us/microsoft-copilot-studio/template-it-helpdesk)

## What it does

- Answers employees' technical questions in natural language, grounded in your organization's ServiceNow knowledge articles.
- When it can't resolve an issue, helps the employee **create a ServiceNow ticket** to escalate to the IT support team.
- Lets employees **look up ticket status** by ticket ID, or list all tickets they submitted through the agent.

## Use cases

- **Self-service troubleshooting** — Resolve common device/software problems from existing knowledge articles without contacting multiple departments.
- **Ticket escalation** — Create a ServiceNow ticket when no article resolves the issue.
- **Ticket tracking** — Check the status of open cases directly through the agent.

## Prerequisites

- A **Copilot Studio** license for your makers.
- Copilot Studio **message capacity**.
- A **ServiceNow** connection and access to an instance with the **knowledge base plugin** enabled (you'll need user credentials and the ServiceNow instance URL).

## How to deploy

1. Open **[Copilot Studio](https://copilotstudio.microsoft.com)** with a Copilot Studio–licensed account.
2. Go to **Agents → New agent → Templates**, then choose **IT Helpdesk**.
3. In the agent's settings, open **Connect your data** and connect **ServiceNow** using your instance URL and credentials.
4. Review the knowledge sources, then **publish** and share the agent with your employees.

## Extension opportunities

- Configure an [engagement hub / hand-off](https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-hand-off) so unresolved conversations escalate to a live support representative with a summary of the issue.
- Add reporting on ticket volumes and response times to help IT managers spot trends.
- Offer self-service actions such as password resets or software installs.

## Limitations

Managed agents and agent templates are currently **English only** and intended for **internal use** within your organization. AI-generated content can contain mistakes — review responses for accuracy. See the [Supplemental Terms](https://go.microsoft.com/fwlink/?linkid=2189520).
