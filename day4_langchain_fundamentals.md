# Day 4 - LangChain Fundamentals

## What is LangChain?

LangChain is an open-source framework that helps developers build applications powered by Large Language Models (LLMs).

It provides components for:

* Prompt management
* Memory
* Chains
* Agents
* Retrieval systems
* Tool integrations

---

## Why LangChain?

Without LangChain, developers often need to manually connect:

1. User Input
2. Prompt Templates
3. LLM Calls
4. Vector Databases
5. External APIs

LangChain simplifies this process through reusable abstractions.

---

## Core Components

### 1. Prompt Templates

Prompt templates allow dynamic prompt generation.

Example:

```python
from langchain.prompts import PromptTemplate

template = PromptTemplate(
    input_variables=["topic"],
    template="Explain {topic} in simple terms."
)

print(template.format(topic="RAG"))
```

---

### 2. Chains

Chains connect multiple operations together.

Example:

User Question → Prompt Template → LLM → Response

---

### 3. Memory

Memory helps applications remember previous interactions.

Types include:

* Conversation Buffer Memory
* Summary Memory
* Entity Memory

---

### 4. Retrievers

Retrievers search relevant information from knowledge bases.

Common retrievers:

* FAISS
* ChromaDB
* Pinecone

---

## Real-World Use Cases

* AI Chatbots
* Customer Support Systems
* Knowledge Base Search
* Document Q&A
* AI Agents

---

## Key Takeaways

* LangChain simplifies LLM application development.
* It provides reusable building blocks.
* It is commonly used with RAG systems.
* Retrievers and memory are essential concepts.
* LangChain helps connect LLMs with external data sources.
