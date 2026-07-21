# BBL AI Engineer Programming Test: Agentic AI

This repository contains a Multi-Agent system implementing a Retrieval-Augmented Generation (RAG) workflow using **LangGraph** and the **Google Gemini API (gemini-2.5-flash)**.

## Repository Contents
- `main.ipynb`: The main Jupyter Notebook containing the multi-agent orchestration code.
- `knowledge_base.txt`: The text file acting as the data source for the RAG system.
- `image_c70153.png`: A screenshot demonstrating the successful execution and final output of the agents.

## Workflow Orchestration
The system orchestrates a sequential workflow with two specialized agents:
1. **Data Retriever Agent**: Uses a custom Python tool to read `knowledge_base.txt` and performs keyword-based chunk retrieval.
2. **Report Generator Agent**: Synthesizes the raw snippets into a well-formatted, non-redundant response using the Gemini 2.5 Flash model.

## Prerequisites
- Google Colab or a local Jupyter Notebook environment.
- Python 3.9+
- A valid Google Gemini API Key.

## How to Run

1. **Open the Notebook:**
   Open `main.ipynb` in your preferred environment (e.g., Google Colab is highly recommended for ease of use).

2. **Install Dependencies:**
   Ensure the following libraries are installed (this is typically included in the first cell of the notebook):
   ```python
   !pip install langgraph langchain-core langchain-google-genai
   ```

3. **Set the API Key:**
   - **If using Google Colab:** Add your Gemini API key to the Colab Secrets (key icon on the left sidebar) and name it `GOOGLE_API_KEY`.
   - **If running locally:** Set it as an environment variable or safely load it within the notebook before initializing the LLM.

4. **Execute:**
   Run all cells sequentially to observe the multi-agent system in action.
