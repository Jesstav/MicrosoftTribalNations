# Microsoft Tribal Nations Community Repository

Welcome to the Microsoft Tribal Nations Community Repository!

This repository is a place for TribalHub members, conference attendees, Microsoft partners, and community contributors to discover, download, share, and improve AI agents created during hackathons, workshops, and community events.

---

# How to Use This Repository

There are two ways to participate:

1. **Browse and download agents** created by others.
2. **Contribute your own agents** and enhancements.

Most users will only need to browse and download content.

---

# Browsing and Downloading Agents

✅ No GitHub experience required

✅ No Fork required

✅ No Pull Request required

✅ In many cases, no GitHub account required

Simply:

1. Open the repository homepage.
2. Browse the folders under `/agents`.
3. Open an agent folder to review its documentation.
4. Download the files you need.

Think of this repository as a community library of AI agents.

---

## Downloading a Single Agent

1. Open the agent's folder.
2. Review the README file.
3. Download the ZIP package or related files.

Example:

```text
agents/
    grants-review-agent/
        README.md
        grants-review-agent.zip
```

The README should explain:

- What the agent does
- How to deploy it
- Requirements or dependencies
- Who created it

---

# Contributing an Agent

If you would like your work published in the repository, you will need to create a Pull Request.

---

# What Is a Pull Request?

A **Pull Request (PR)** is GitHub's review process.

Think of it as saying:

> "I'd like to contribute these files to the community repository. Please review them before publishing."

Your contribution will be reviewed by repository maintainers before it is merged into the shared repository.

---

# Step 1: Create a GitHub Account

If you do not already have one:

1. Visit https://github.com
2. Select **Sign Up**
3. Complete registration
4. Verify your email address

---

# Step 2: Create a Fork

Open the repository homepage.

In the upper-right corner, click:

```text
Fork
```

A Fork is your personal copy of the repository.

This allows you to make changes without affecting the main repository.

---

# Step 3: Create a Folder for Your Submission

Within your Fork:

Navigate to:

```text
agents/
```

Create a new folder using a descriptive name.

Example:

```text
agents/
    permit-review-assistant/
```

Avoid folder names such as:

```text
newagent
team7
finalversion
hackathon
```

Use names that clearly describe the purpose of the agent.

---

# Step 4: Upload Your Files

Upload the materials needed to use your agent.

Recommended contents:

```text
agents/
    permit-review-assistant/
        README.md
        permit-review-assistant.zip
        screenshot1.png
        screenshot2.png
```

At a minimum, include:

- Agent package or ZIP file
- README documentation

---

# Step 5: Create a README

Each submission should include a file named:

```text
README.md
```

Use the following template:

```markdown
# Permit Review Assistant

## Summary

Assists staff with permit review workflows.

## Created By

Jane Smith

## Event

TribalHub AI Hackathon 2026

## Technologies Used

- Microsoft Copilot Studio
- Azure OpenAI
- Power Automate

## Features

- Reviews permit applications
- Identifies missing information
- Answers policy questions

## Deployment Instructions

1. Import the package.
2. Configure connections.
3. Test using sample data.

## Requirements

- Microsoft 365
- Copilot Studio License
```

---

# Step 6: Commit Your Changes

After uploading your files:

Scroll to the bottom of the page.

Enter a short description.

Example:

```text
Added Permit Review Assistant
```

Click:

```text
Commit Changes
```

A **Commit** is simply GitHub's term for saving your changes.

---

# Step 7: Create a Pull Request

After committing:

1. Click **Contribute**
2. Click **Open Pull Request**

GitHub will display a summary of everything you added or changed.

---

# Step 8: Describe Your Submission

Provide a short summary.

Example:

```text
This submission contains a permit review assistant created during the TribalHub AI Hackathon.

Features:
- Permit review guidance
- Policy lookup
- Automated recommendations

Created by Jane Smith.
```

Click:

```text
Create Pull Request
```

Your submission is now ready for review.

---

# What Happens Next?

Repository maintainers will review your submission.

They may:

- Approve it
- Ask questions
- Request additional documentation
- Suggest improvements

Once approved, your contribution will be merged into the repository and made available to the community.

---

# Agent Types in This Repository

This gallery holds two kinds of Microsoft Copilot agents. Which files you include depends on the type:

- **M365 Copilot (Agent Builder)** — declarative agents you build by pasting an *Instructions* block and a *Description* into [Copilot Agent Builder](https://copilot.microsoft.com). These ship with `instructions.txt` + `description.txt` alongside the README.
  - Keep `instructions.txt` **at or under 8,000 characters** (Agent Builder's limit). Verify the count before submitting.
  - Add a concise one-paragraph `description.txt`.
- **Copilot Studio (template or exported solution)** — agents you install/import and configure in [Copilot Studio](https://copilotstudio.microsoft.com). Document these with a `README.md`; include an importable `.zip` only when it contains **no secrets, tokens, internal URLs, or customer data** (sanitize or ship instructions-only otherwise).

After adding your agent folder, **add a row to the Agents table in the top-level [`README.md`](./README.md)** so it shows up in the gallery index.

## Attribution & Licensing

- This repo is **MIT-licensed** (see [`LICENSE`](./LICENSE)).
- If your agent is **adapted from a community sample** (e.g., [pnp/copilot-prompts](https://github.com/pnp/copilot-prompts)), credit the **original author and source** in the agent's `README.md`. Only contribute content you have the right to share.
- If your agent is **original**, note that it was built for this gallery.

## Respectful Language

Prefer inclusive, respectful language. For agents intended for Tribal Nations audiences, use preferred names and terminology and avoid stereotypes.

---

# Best Practices

## Include Documentation

Submissions without documentation are difficult for others to use.

Always include:

- Description
- Deployment instructions
- Requirements
- Contact information (optional)

---

## Use Descriptive Names

Good:

```text
records-management-assistant
grant-review-agent
tribal-policy-search
```

Avoid:

```text
agent1
final
newversion
team3
```

---

## Remove Sensitive Information

Before uploading:

- Remove passwords
- Remove API keys
- Remove connection strings
- Remove customer data
- Remove personal information

Anything submitted to a public repository may be visible to others.

---

## Upload Working Versions

Please test your agent before submission.

If the project is experimental, note that in the README.

---

# GitHub Terms Explained

| Term | Meaning |
|--------|----------|
| Repository | The shared community library |
| Fork | Your personal copy of the repository |
| Folder | A location where files are stored |
| Commit | Save your changes |
| Pull Request | Request that your changes be reviewed and added |
| Review | Feedback from repository maintainers |
| Merge | Approval and publication of your contribution |

---

# Frequently Asked Questions

## Do I need a GitHub account to browse the repository?

Usually no.

Most public repositories can be viewed and downloaded without signing in.

---

## Do I need a Fork to download files?

No.

Forks are only needed when you want to contribute changes.

---

## Do I need a Pull Request to download files?

No.

Pull Requests are only used when submitting content for review.

---

## Can I update an existing agent?

Yes.

Create a Fork, make your changes, and submit a Pull Request explaining the update.

---

## Can I contribute more than once?

Absolutely.

Community contributions are encouraged.

---

# Quick Summary

### To Download an Agent

1. Open the repository.
2. Browse the `/agents` folder.
3. Download what you need.

No Fork required.
No Pull Request required.

### To Contribute an Agent

1. Create a GitHub account.
2. Fork the repository.
3. Upload your files.
4. Commit your changes.
5. Create a Pull Request.
6. Wait for review and approval.

Thank you for helping build the TribalHub AI Community!
