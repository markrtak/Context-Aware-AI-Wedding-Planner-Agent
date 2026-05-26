# Multi-Agent Wedding Planner with LangChain

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-121212?style=for-the-badge)
![Tavily](https://img.shields.io/badge/Tavily-AI_Search-blue?style=for-the-badge)
![RAG](https://img.shields.io/badge/RAG-Knowledge_Base-darkgreen?style=for-the-badge)
![MCP](https://img.shields.io/badge/MCP-Tool_Protocol-purple?style=for-the-badge)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge\&logo=sqlite\&logoColor=white)

## Overview

This project demonstrates a multi-agent AI wedding planner capable of coordinating wedding-related workflows using LangChain agents, Tavily search, RAG pipelines, MCP integrations, and structured tool execution.

The system uses a coordinator-driven multi-agent architecture where a central coordinator agent manages multiple specialized subagents responsible for different wedding planning workflows.

The assistant supports workflows such as:

* Wedding planning coordination
* Venue and destination research
* Timeline planning
* Budget recommendations
* Music and playlist querying
* Knowledge base retrieval
* Real-time web research
* Multi-step agent collaboration

---

## Features

* Multi-agent workflow orchestration
* Coordinator and specialized subagent architecture
* Tavily-powered AI web search and retrieval
* RAG-based wedding planning knowledge base
* MCP tool integration
* SQLite database querying
* Context-aware conversational workflows
* Structured tool calling
* Wedding planning recommendation system
* Retrieval-augmented generation pipeline
* LangChain agent coordination
* Error-handled MCP execution

---

## Architecture

```text
User Request
      │
      ▼
Coordinator Agent
      │
      ├── Wedding Planning Subagent
      ├── Venue Research Subagent
      ├── Budget Planning Subagent
      ├── Playlist Recommendation Subagent
      ├── Tavily Search Integration
      ├── RAG Knowledge Base
      ├── MCP Tool Layer
      └── SQLite Playlist Database
                    │
                    ▼
         Wedding Planning Response
```

---

## Installation

Install the required dependencies:

```bash
pip install langchain tavily-python python-dotenv langchain-community langchain-mcp-adapters sqlite3
```

---

## Environment Variables

Create a `.env` file:

```env
TAVILY_API_KEY=your_api_key_here
GROQ_API_KEY='groq_api_key'
```

---

## Core Components

### Coordinator Agent

The coordinator agent is responsible for:

* Task delegation
* Workflow routing
* Agent coordination
* Response aggregation
* Tool orchestration
* Managing communication between subagents

---

### Specialized Subagents

The system uses multiple specialized subagents responsible for different wedding planning workflows.

Supported subagent workflows include:

* Wedding planning
* Venue research
* Budget recommendations
* Playlist retrieval
* Web search
* Knowledge retrieval

---

### Tavily Integration

Tavily is integrated as the primary AI-powered web search and retrieval system.

The agents use Tavily workflows for:

* Wedding destination research
* Vendor discovery
* Venue information lookup
* Planning recommendations
* Real-time information retrieval
* External knowledge access

---

### RAG Knowledge Base

The system includes a retrieval-augmented generation pipeline containing wedding planning knowledge and expert guidance.

The RAG workflow supports:

* Timeline recommendations
* Budget guidance
* Wedding best practices
* Planning checklists
* Destination wedding advice
* Personalized retrieval workflows

---

### MCP Tool Integration

The project integrates MCP-compatible tools using a MultiServer MCP client architecture.

The workflow includes:

* MCP tool execution
* Retry handling
* Structured tool responses
* Error recovery pipelines
* External tool coordination

---

### SQLite Database Integration

The assistant includes database querying capabilities using SQLite.

Database workflows include:

* Playlist querying
* Music recommendation support
* Structured data retrieval
* SQL-powered planning utilities

---

## RAG Workflow

```text
Wedding Documents
        │
        ▼
Text Splitting
        │
        ▼
Embedding Generation
        │
        ▼
Vector Store Indexing
        │
        ▼
Similarity Search
        │
        ▼
Retrieved Context for Agents
```

---

## Multi-Agent Workflow

```text
1. User submits wedding planning request
2. Coordinator agent routes the task
3. Specialized subagents process their responsibilities
4. Tavily retrieves external information
5. RAG pipeline retrieves wedding knowledge
6. MCP tools execute structured operations
7. SQLite queries retrieve playlist information
8. Coordinator agent aggregates the final response
```

---

## Tech Stack

| Technology       | Purpose                         |
| ---------------- | ------------------------------- |
| Python           | Core application development    |
| LangChain        | Multi-agent orchestration       |
| Tavily           | AI-powered search and retrieval |
| MCP              | Tool protocol integration       |
| SQLite           | Structured database querying    |
| RAG Pipeline     | Knowledge retrieval workflows   |
| Vector Store     | Semantic document retrieval     |
| dotenv           | Environment management          |
| Jupyter Notebook | Interactive experimentation     |

---

## Future Improvements

* Persistent long-term memory
* Vendor booking automation
* Calendar integrations
* Real-time collaboration workflows
* Budget optimization agents
* Email automation
* AI-generated wedding itineraries
* Multi-user planning support
* Voice-enabled planning assistant

---

## Result

This project provides a foundation for building production-ready coordinator-driven multi-agent AI systems capable of:

* Intelligent workflow orchestration
* Retrieval-augmented reasoning
* Real-time search integration
* MCP tool execution
* Structured database querying
* Multi-agent collaboration
* Context-aware planning systems
