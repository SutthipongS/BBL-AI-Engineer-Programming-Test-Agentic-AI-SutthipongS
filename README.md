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
1. Install dependencies:
   ```bash
   pip install langgraph langchain-core langchain-google-genai
Set your Google Gemini API key as an environment variable (or within the script).

Run the orchestration script:
