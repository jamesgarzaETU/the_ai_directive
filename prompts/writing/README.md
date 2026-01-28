# ✍️ Writing & Documentation

**Focus:** Internal documentation, emails to stakeholders, and release notes.

## 🧱 Best Practices
1.  **Load Context First:** Upload `context/project_specs.md` (Auto Insights Modernization) before drafting.
2.  **Define the Audience:**
    * **Executive:** Conor, Gordon (Focus on ROI, Speed, Security).
    * **Technical:** Jeremy, Dev Team (Focus on S3 Structure, Dependencies).

## 📋 Prompt Catalog

### 1. The "Technical Brief Generator"
**Use when:** Preparing the requirements document for Jeremy.
> "Draft a Technical Brief for [Project Name].
>
> **Context:**
> - Goal: Modernize data pipeline to S3/Parquet.
> - Current Pain Point: 80% of time spent on maintenance/loading.
> - Deliverable: A finalized `pipeline_modernization.md` spec.
>
> **Structure the Brief with:**
> 1. Problem Statement.
> 2. Proposed Architecture (Diagram description).
> 3. Definition of Success (Speed < 10 mins).
> 4. Questions for the Technical Lead."

### 2. The "Stakeholder Buy-In Pitch"
**Use when:** Emailing Conor and Gordon to approve the new architecture.
> "Draft an update email for Executive Stakeholders.
> **Key Message:** We are switching to a 'Data Lake' model to reduce reporting time by 90%.
> **Tone:** Confident, strategic, high-level.
> **Ask:** Approval to proceed with Phase 1 (Infrastructure Setup).
>
> Highlight that this satisfies the Annual Goal regarding 'Scalable Platforms'."

### 3. The "Readme Generator"
**Use when:** Documenting new scripts (e.g., `parquet_pipeline.py`).
> "Write a `README.md` for the following Python script. Include prerequisites (libraries) and usage examples."
