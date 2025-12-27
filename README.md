# 📊 CSV Chat Agent with Google Gemini & LangChain

An intelligent data analysis agent that allows you to "chat" with your CSV data using natural language. Built with **Google Gemini (GenAI)**, **LangChain**, and **Python**.

## 🚀 Features

* **Natural Language Queries:** Ask questions like "What is the average salary?" or "Who is the oldest employee?"
* **Data Visualization:** Automatically generates Bar Charts and Pie Charts using Matplotlib based on your text prompts.
* **Multi-step Reasoning:** Uses LangChain's CSV Agent to perform complex filtering, aggregation, and segmentation.
* **Powered by Gemini:** Utilizes the `gemini-1.5-flash` (or 2.5) model for high-speed, low-cost reasoning.

## 🛠️ Tech Stack

* [LangChain](https://www.langchain.com/) - Orchestration framework.
* [Google Gemini API](https://ai.google.dev/) - LLM backend.
* [Pandas](https://pandas.pydata.org/) - Data manipulation.
* [Matplotlib](https://matplotlib.org/) - Graphing and visualization.

## 📋 Prerequisites

1.  Python 3.10+
2.  A Google AI Studio API Key. Get one [here](https://aistudio.google.com/).

## ⚙️ Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/ergaikwadketan/gemini-csv-agent.git](https://github.com/ergaikwadketan/gemini-csv-agent.git)
    cd gemini-csv-agent
    ```

2.  **Install dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Set up your API Key:**
    Open the notebook and locate the cell:
    ```python
    os.environ["GOOGLE_API_KEY"] = "YOUR_API_KEY_HERE"
    ```
    *Note: For production use, it is recommended to use a `.env` file rather than hardcoding keys.*

## 🏃‍♂️ Usage

1.  Open the Jupyter Notebook:
    ```bash
    jupyter notebook csv_chat_agent_tool_gemini.ipynb
    ```
2.  Run the cells sequentially.
3.  The notebook creates a dummy dataset (`employees.csv`) automatically.
4.  Scroll to the **"Execute Queries"** section to see the agent in action.

## 🧠 Example Queries

The agent handles various complexities:

* **Simple:** "How many total employees are there?"
* **Conditional:** "How many people have the letter 'n' in their name and work in Marketing?"
* **Analytical:** "Compare the top 2 highest-paid departments."
* **Visual:** "Create a pie chart department wise in percentage of employee."

## ⚠️ Security Note

This project uses `allow_dangerous_code=True` in the LangChain CSV Agent. This enables the LLM to execute Python code to analyze data. Only run this on trusted CSV files and in a sandboxed environment.

## 📄 License

MIT License

***
## Created By Ketan Dilip Gaikwad
