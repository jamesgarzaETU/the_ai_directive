# ✍️ Writing & Documentation

**Focus:** Internal documentation, emails to stakeholders, and release notes.

## 🧱 Best Practices
1.  **Load Context First:** Before asking for a draft, upload `context/brand_voice.md` or `context/project_specs.md`.
2.  **Define the Audience:** Explicitly state if this is for "Technical Developers" (details okay) or "Executive Stakeholders" (high-level only).

## 📋 Prompt Catalog

### 1. The "Stakeholder Update"
**Use when:** Explaining technical delays or wins to non-technical leadership (e.g., Conor/Gordon).
> "Draft a weekly update email based on the bullet points below.
> Tone: Professional, concise, solution-oriented.
> Audience: Non-technical executive stakeholders.
>
> Key Points:
> - [Insert Achievement, e.g., S3 Bucket setup complete]
> - [Insert Blocker, e.g., Waiting on API access]
> - [Insert Next Step]"

### 2. The "Readme Generator"
**Use when:** You've written a script but haven't documented it.
> "Write a `README.md` for the following Python script.
> Include:
> - 'Prerequisites' section (libraries used).
> - 'Usage' section with a command line example.
> - A brief explanation of what the script does.
>
> [Paste Code Here]"

### 3. The "Technical Spec Polish"
**Use when:** Your rough notes need to become a formal Jira ticket or design doc.
> "Rewrite these rough notes into a structured Technical Specification. Use the following headers: 'Objective', 'Technical Approach', 'Risks', and 'Definition of Done'."
