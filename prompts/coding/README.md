# 💻 Coding Prompts

**Focus:** Code generation, refactoring, unit testing, and technical documentation.

## 🧱 Best Practices
1.  **Define the Stack:** Explicitly state: "Python 3.9+, Pandas, **PyArrow**, AWS SDK (Boto3)."
    * *Note: We are moving away from raw SQL queries.*
2.  **Paste the Interface:** If writing a function that interacts with S3, provide the bucket structure (`raw_tables`, `metadata`).
3.  **One Task at a Time:** Don't ask for "Refactor this and add a new feature." Do them in separate turns.

## 📋 Prompt Catalog

### 1. The "SQL to Parquet Migrator"
**Use when:** converting legacy `Auto Insights` SQL queries into efficient Pandas transformations.
> "I have a legacy SQL query that performs the following joins/aggregations. Rewrite this logic using Python and Pandas.
>
> **Constraints:**
> - Input data is loaded from Parquet files (not a DB connection).
> - Use vectorization (avoid `apply` where possible).
> - Ensure output types match the target schema.
>
> [Paste Legacy SQL Query Here]"

### 2. The "Unit Test Generator"
**Use when:** Improving test coverage for critical logic (e.g., `update_table_incremental`).
> "I have the following function `[Insert Function Name]`. Please write a `pytest` suite for it.
>
> Include test cases for:
> 1. Happy path (standard input).
> 2. Edge cases (null values, empty lists).
> 3. **Mocking S3 calls** (using `moto` or mock objects).
>
> [Paste Function Code Here]"

### 3. The "Clean Refactor"
**Use when:** Optimizing legacy code.
> "Refactor the following Python code to adhere to PEP8 standards. Optimize for readability and memory usage. Do not change the external behavior."
