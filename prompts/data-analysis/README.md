# 📊 Data Analysis & SQL

**Focus:** SQL generation, Pandas transformations, and Plotly visualization logic.

## 🛑 SAFETY WARNING
**NEVER PASTE REAL CUSTOMER DATA (PII) INTO THE CHAT.**
* **Do:** Paste column headers (schema) or fake sample rows.
* **Don't:** Paste user emails, IDs, or raw financial logs.

## 🧱 Best Practices
1.  **Schema First:** Always provide the `CREATE TABLE` statement or the output of `df.info()` so the AI understands the data structure.
2.  **Specify the Dialect:** PostgreSQL syntax differs from MySQL. Be specific.

## 📋 Prompt Catalog

### 1. The "Complex SQL Builder"
**Use when:** You need a complex join or window function.
> "Write a MySQL query to calculate the [Metric, e.g., Monthly Retention Rate].
>
> Table Schema:
> - users (id, signup_date)
> - activity_log (user_id, timestamp, action_type)
>
> Requirements:
> - Group by month.
> - Filter out 'admin' users.
> - Use a CTE for readability."

### 2. The "Plotly Dashboard Helper"
**Use when:** Converting D3.js or static charts to Python Plotly (for the Modernization project).
> "Write a Python function using `plotly.graph_objects` to visualize this dataframe.
>
> Dataframe columns: `[date, usage_count, user_segment]`
> Visualization type: Stacked Bar Chart.
> Style: Minimalist, white background.
>
> Ensure the layout is responsive."

### 3. The "Regex Extractor"
**Use when:** Cleaning messy string data in Pandas.
> "Write a Python Regex pattern to extract the transaction ID (format: 'TXN-1234') from the following raw log strings. Then show me how to apply it to a Pandas column named `raw_logs`."
