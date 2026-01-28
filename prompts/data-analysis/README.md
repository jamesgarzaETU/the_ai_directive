# 📊 Data Analysis & SQL

**Focus:** SQL generation, Pandas transformations, and Plotly visualization logic.

## 🛑 SAFETY & PERFORMANCE WARNING
1.  **NO PII:** Never paste real customer names/emails.
2.  **NO DIRECT DB HITS:** The goal is to move analysis to S3. **Do not generate code that queries the production MySQL DB for analytics.** Always query the local Parquet files.

## 📋 Prompt Catalog

### 1. The "Plotly Modernizer"
**Use when:** Converting old D3.js or Static Images to interactive Plotly charts.
> "Write a Python function using `plotly.graph_objects` to visualize this dataframe.
>
> **Requirements:**
> - Input: Pandas DataFrame (from Parquet).
> - Style: Minimalist, White Background (match Brand CSS).
> - Interactivity: Enable hover states for detailed metrics.
> - **Output:** A standalone HTML component or JSON for the dashboard.
>
> [Describe the Chart Needed]"

### 2. The "Parquet Optimizer"
**Use when:** Determining how to save data efficiently.
> "Suggest the best partitioning strategy for this dataset in Parquet format.
>
> **Columns:** `[date, user_id, simulation_id, score]`
> **Query Pattern:** We usually filter by `simulation_id` and then `date`.
>
> Tell me how to structure the `partition_cols` argument in `pyarrow`."

### 3. The "Regex Extractor"
**Use when:** Cleaning messy log strings in Pandas.
> "Write a Python Regex pattern to extract specific IDs from raw logs."
