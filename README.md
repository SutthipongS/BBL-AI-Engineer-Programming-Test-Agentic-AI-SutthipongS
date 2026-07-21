# BBL AI Engineer Programming Test: Agentic AI

This repository contains a Multi-Agent system implementing a Retrieval-Augmented Generation (RAG) workflow using **LangGraph** and the **Google Gemini API (gemini-2.5-flash)**.

## Workflow Orchestration
The system orchestrates a sequential workflow with two specialized agents:
1. **Data Retriever Agent**: Uses a custom Python tool to read `knowledge_base.txt` and performs keyword-based chunk retrieval.
2. **Report Generator Agent**: Synthesizes the raw snippets into a well-formatted, non-redundant response using the Gemini 2.5 Flash model.

## Prerequisites
- Python 3.9+
- A valid Google Gemini API Key

## How to Run

1. **Install required dependencies:**
```bash
pip install langgraph langchain-core langchain-google-genai
```

2. **Set your Google Gemini API Key:**
The system requires a valid Gemini API key to function. Please set it as an environment variable using your terminal before running the script.

* For **Mac/Linux**:
```bash
export GOOGLE_API_KEY="your_api_key_here"
```

* For **Windows (Command Prompt)**:
```cmd
set GOOGLE_API_KEY="your_api_key_here"
```

* For **Windows (PowerShell)**:
```powershell
$env:GOOGLE_API_KEY="your_api_key_here"
```
   
*(Note: Alternatively, you can temporarily hardcode the key in `main.py` for quick testing, but using environment variables is highly recommended).*

3. **Run the orchestration script:**
```bash
python main.py
```
