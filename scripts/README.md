# ⚡ Automation Scripts

This folder contains Python and Node.js scripts for interacting with AI APIs (OpenAI, Anthropic, Gemini, etc.) programmatically.

## ⚠️ Security Warning
* **NEVER commit API keys.**
* Always use a `.env` file to store secrets.
* Ensure `.env` is listed in your `.gitignore`.

## 🛠️ Setup Guide

1.  **Clone the repo:**
    ```bash
    git clone [repo-url]
    ```

2.  **Create Virtual Environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # (Windows: venv\Scripts\activate)
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Configure Environment:**
    Rename `.env.example` to `.env` and add your keys:
    ```text
    OPENAI_API_KEY=sk-...
    ANTHROPIC_API_KEY=sk-...
    ```
