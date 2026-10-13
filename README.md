# 🤖 LangGraph Agentic RAG System with Groq LLM

An enterprise-ready **Agentic AI Workflow** built using **LangGraph**, **LangChain**, and **Groq LLM**. The agent dynamically decides when to query internal enterprise knowledge base tools and synthesizes responses based on state-aware message graphs.

---

## 🏗️ Architecture & Workflow

The system utilizes a directed cyclic graph (DAG) with condition-based tool routing:

1. **State Management**: Uses `MessagesState` to store and track full conversation history.
2. **Conditional Routing**: Evaluates `tool_calls` in the model response to route execution dynamically.
3. **Internal Knowledge Integration**: Custom `@tool` execution for company report retrieval.

---

## 🛠️ Tech Stack

* **Orchestration**: LangGraph, LangChain Core
* **LLM Engine**: Groq API (`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`)
* **Environment**: Jupyter Notebook / Python 3.10+

---

## 🚀 How to Run

1. Open `LangGraph_Agentic_AI_Workflow.ipynb` in Google Colab or Jupyter Notebook.
2. Set your `GROQ_API_KEY` when prompted.
3. Run all cells sequentially to execute the agent graph.

---

## 📊 Sample Output

```text
User Query: "What is our Q3 revenue?"
[Agent Action]: Executing tool 'search_internal_knowledge'
[Tool Response]: Internal Knowledge Base Results for 'What is our Q3 revenue?'...

--- AI Response ---
Based on our internal documents, the company's Q3 revenue grew by 15%, driven by advanced AI automation workflows.
