# ReAct-RAG-Data-Analyst-Agent
Fabric + ReAct + RAG

## Overview
This project builds an AI-powered autonomous data analyst capable of answering business questions using multiple data sources and intelligent reasoning.
Instead of following a fixed pipeline, the system uses a ReAct (Reason + Act) agent that dynamically decides how to answer a query.
The agent combines:

Structured data (Microsoft Fabric Lakehouse)
Internal knowledge (RAG)
External knowledge (Wikipedia)
AI reasoning (LLM)

------
## Architecture

<img width="1536" height="1024" alt="Designer (22)" src="https://github.com/user-attachments/assets/99325eab-05ba-4ecb-93ce-5d0ea451193b" />

-----

## System Flow

  1. User asks a natural language question
  2. ReAct Agent analyzes the intent
  3. Agent selects appropriate tool(s)
  4. Data is retrieved or analyzed
  5. Outputs are combined
  6. Final answer with insights is generated
-----
## Key Concepts
## ReAct Agent (Reason + Act)
The core intelligence of the system.
Instead of a fixed sequence, the agent:

Thinks before acting
Chooses tools dynamically
Iterates if needed

This enables human-like analytical reasoning.

-------

## Multi-Tool Architecture
The agent has access to multiple tools and selects the best one depending on the query.

### SQL Tool
Queries structured data from Microsoft Fabric
Used for counts, filters, trends

### Python Tool
Analyzes data outputs
Generates insights, comparisons, patterns

### RAG Tool (Retrieval-Augmented Generation)
Retrieves internal knowledge from documents
Enables organization-specific context

### Wikipedia Tool
Provides external knowledge
Used for explanations, trends, and reasoning

-------

## Retrieval-Augmented Generation (RAG)
RAG enhances the system by allowing it to use internal documents as a knowledge source.
### Flow:

  - Store documents (PDFs, reports)
  - Retrieve relevant content
  - Generate contextual answers

This ensures:

  - Context-aware insights
  - Business-specific reasoning

------

## Natural Language to SQL
The system automatically converts user questions into SQL queries.
Example:
# User:
“How many tickets were created last month?”
# System:
Generates SQL → Executes on Fabric → Returns results
This removes dependency on manual querying.

-------

## AI-Based Data Analysis
Beyond retrieving data, the system:

  - Interprets results
  - Identifies patterns
  - Explains trends

It behaves like a data analyst, not just a query engine.

### Example Query Flow
### Question:
“Why do tickets increase during holidays?”
### Agent behavior:

  - Identifies need for explanation
  - Uses Wikipedia for general trends
  - Uses RAG for internal context
  - Combines insights
  - Produces final explanation

-------

## Features

  - Natural language query interface
  - Autonomous tool selection
  - Multi-source reasoning
  - Context-aware responses
  - Internal + external knowledge integration
  - Explainable AI output

-------

## Use Cases

  - Business analytics assistant
  - Customer support insights
  - Operational intelligence
  - Decision support systems
  - AI copilots for data teams

--------

## Tech Stack

  - Microsoft Fabric (Lakehouse)
  - LangChain (ReAct agent framework)
  - OpenAI LLM
  - ChromaDB (for RAG)
  - Wikipedia API

--------

## Summary
This project showcases how modern AI systems are built by combining:

  - Data engineering
  - AI reasoning
  - Knowledge retrieval
  - Tool orchestration

It reflects real-world AI architectures used in:

  - Enterprise copilots
  - Intelligent assistants
  - Autonomous analyst systems

------


## Author

Supriya Singh

 AI & Data Engineer



