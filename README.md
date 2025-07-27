# 🧠 LangGraph Exploration – Agentic LLM Workflows

This repository showcases hands-on experiments with [LangGraph](https://github.com/langchain-ai/langgraph), an extension of LangChain for building **stateful, multi-agent LLM applications** using a graph-based approach.

## 🔍 What is LangGraph?
LangGraph allows you to define dynamic, branching, and looping workflows for LLM applications — making it ideal for:
- Agent orchestration with memory and tools
- Conditional logic and retry handling
- Multi-step GenAI pipelines

## 🚀 What's Inside
- `01_hello_langgraph`: Minimal working example with a single LLM node
- `02_branching_graph`: Conditional node routing using user input
- `03_multi_agent_loop`: Crew-style agents with memory and looping
- `04_rag_pipeline`: Retrieval-augmented generation using LangGraph
- `utils/`: Shared code, configs, and helper functions

## ⚙️ Tech Stack
- LangGraph + LangChain
- OpenAI / Gemini (LLMs)
- ChromaDB / Weaviate (Vector DB)
- CrewAI (for agent composition)
- Python 3.10+

## 📦 Setup

```bash
# Clone the repo
git clone https://github.com/yourusername/langgraph-experiments.git
cd langgraph-experiments

# Create and activate virtual environment using uv
uv venv .venv
source .venv/bin/activate  # macOS/Linux
# .venv\Scripts\activate     # Windows

# Install dependencies
uv pip install -r requirements.txt

# (Optional) Add venv to JupyterLab kernel
uv pip install ipykernel
python -m ipykernel install --user --name=langgraph-env --display-name "LangGraph (uv venv)"
