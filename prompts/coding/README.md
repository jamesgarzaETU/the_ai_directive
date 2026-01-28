# 💻 Coding Prompts

**Focus:** Code generation, refactoring, unit testing, and technical documentation.

## 🧱 Best Practices
1.  **Define the Stack:** Always specify "Python 3.9+, Pandas, AWS Lambda" to avoid getting generic or outdated code.
2.  **Paste the Interface:** If writing a function that interacts with another class, paste the method signature/interface of that class first.
3.  **One Task at a Time:** Don't ask for "Refactor this and add a new feature." Do them in separate turns.

## 📋 Prompt Catalog

### 1. The "Clean Refactor"
**Use when:** Optimizing legacy code (e.g., modernizing the old SQL pipeline).
> "Refactor the following Python code to adhere to PEP8 standards. Optimize for readability and memory usage. Do not change the external behavior or return values.
>
> Constraints:
> - Use type hinting.
> - Add docstrings (Google Style).
> - Replace `for` loops with vectorization where possible (Pandas)."

### 2. The "Unit Test Generator"
**Use when:** Improving test coverage for critical logic.
> "I have the following function `[Insert Function Name]`. Please write a `pytest` suite for it.
>
> Include test cases for:
> 1. Happy path (standard input).
> 2. Edge cases (null values, empty lists).
> 3. Error handling (expected exceptions).
>
> [Paste Function Code Here]"

### 3. The "Bug Hunter"
**Use when:** You have a stack trace but don't see the logical error.
> "Analyze this error log and the accompanying code snippet. Explain the root cause of the `KeyError` and suggest a defensive coding fix."
