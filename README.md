# 🛠️ Codeforge

**Codeforge** is an AI-powered software agent that transforms natural language requests into complete, working projects. Built on [LangGraph](https://github.com/langchain-ai/langgraph), it operates like a multi-agent development team, tackling complex tasks by using real-world developer workflows to create projects file by file.

---

### ✨ Key Features

* **Multi-Agent System:** Employs a specialized team of AI agents for planning, architecture, and coding.
* **Developer Workflow:** Mimics a human development process, from high-level planning to file-specific implementation.
* **End-to-End Generation:** Delivers a complete, functional project from a single prompt, ready to run.

---

## 🏗️ Architecture

Codeforge's core power comes from its three specialized agents, each handling a critical phase of the development lifecycle:

* **Planner Agent**
    * Analyzes your request and generates a detailed, high-level project plan.

* **Architect Agent**
    * Decomposes the overall plan into a series of granular engineering tasks, providing explicit context for each file.

* **Coder Agent**
    * Executes each task by reading, writing, and modifying files, acting as the hands-on developer to build the project piece by piece.

---

## 🚀 Getting Started

### Prerequisites
* **Python 3.x:** Ensure you have Python(3.11 in this case) and `pip` installed.
* **Groq API Key:** You will need an API key from Groq. Create one [here](https://console.groq.com/keys).

### ⚙️ Installation and Setup
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/your-repo-name/codeforge.git](https://github.com/your-repo-name/codeforge.git)
    cd codeforge
    ```
2.  **Create and activate your virtual environment:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    ```
3.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Configure your API key:**
    * Copy the example environment file:
        ```bash
        cp .sample_env .env
        ```
    * Open the newly created `.env` file and add your Groq API key:
        ```
        GROQ_API_KEY=your_api_key_here
        ```
5.  **Run the application:**
    ```bash
    python main.py
    ```

---

### 🧪 Example Prompts

Here are some ideas to get you started. Provide your prompt directly to the `main.py` script.

* `Build a colourful modern to-do app using HTML, CSS, and JavaScript.`
* `Create a simple calculator web application.`
* `Create a simple blog API in FastAPI with a SQLite database.`