# NeuroFetch: Deep Research AI Agentic System

NeuroFetch is a modular, dual-agent AI system designed for automated web-based research and intelligent answer generation. By integrating **Tavily** for web crawling and **LangGraph** with **LangChain** for structured agent coordination, the system provides a robust and scalable solution for real-time information gathering and contextual response generation.

---

## 📌 Key Features

- **Dual-Agent Architecture**  
  - *Research Agent:* Conducts online research and gathers relevant information using Tavily.  
  - *Answer Drafting Agent:* Synthesizes accurate, structured, and fluent responses from parsed data.

- **LangGraph-based Flow Control:** Enables deterministic agent orchestration, state transitions, and retry logic.

- **LangChain Integration:** Facilitates workflow execution through prompt templates and modular chain definitions.

- **Web-Scale Research Capability:** Retrieves and processes real-time data from publicly accessible websites.

- **Customizable and Scalable Design:** Supports easy extension to additional agents or use cases.

---

## 📐 System Architecture

```mermaid
graph TD
    A[User Query Input] --> B[Research Agent]
    B --> C[Tavily API - Web Crawling]
    C --> D[Data Parsing and Filtering]
    D --> E[Answer Drafting Agent]
    E --> F[Response Generation (LangChain)]
    F --> G[Final Output to User]
