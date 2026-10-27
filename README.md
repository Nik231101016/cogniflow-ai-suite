# 🚀 CogniFlow AI Suite (n8n Multi-Agent & Automation Workflows)

An advanced collection of production-ready **n8n workflows** powered by Large Language Models (LLMs), LangChain, Vector Databases, and automated integrations. This repository bridges the gap between traditional workflow automation and autonomous AI agents to streamline business operations like customer support, email routing, document extraction, and error handling.

---

## 📋 Table of Contents
- [Core Workflows Included](#-core-workflows-included)
- [Tech Stack & Integrations](#-tech-stack--integrations)
- [Architecture Overview](#-architecture-overview)
- [Setup & Installation](#-setup--installation)
- [Usage Guidelines](#-usage-guidelines)
- [Credits](#-credits)

---

## 🛠️ Core Workflows Included

### 1. Intelligent Email Router & Specialized Agents (`17) Routing.json`)
* **Description:** Eliminates generalist AI bottlenecks by classifying incoming emails and routing them to specialized department agents.
* **Categories & Routing:**
  * **High Priority:** Summarizes urgent requests and triggers real-time **Telegram** alerts.
  * **Customer Support:** Handles client inquiries professionally, signing off as a designated support rep.
  * **Promotions:** Manages marketing and partnership proposals.
  * **Finance/Billing:** Handles payment, invoice, and receipt inquiries.

### 2. RAG Workflow vs. RAG Agent (`11) RAG Workflow vs RAG Agent.json`)
* **Description:** Demonstrates and implements Retrieval-Augmented Generation (RAG) using vector databases.
* **Features:**
  * Automated document ingestion, text splitting (Recursive Character Text Splitter), and embedding generation via **OpenAI**.
  * Vector storage and semantic search via **Pinecone**.
  * Configured as both an automated workflow and an interactive customer support agent tool.

### 3. Automated Invoice Processing (`4) Invoice Workflow.json`)
* **Description:** End-to-end invoice automation pipeline.
* **Workflow Steps:**
  * Triggers on new PDF uploads in **Google Drive**.
  * Extracts text and uses **Google Gemini** as an information extraction engine to pull structured attributes (Invoice Number, Client Name, Amounts, Dates).
  * Automatically updates tracking logs and notifies the internal billing team via **Gmail**.

### 4. Global Error Logger & Monitoring (`21) Error Logger.json`)
* **Description:** Global error handling workflow to ensure high system reliability.
* **Features:**
  * Automatically catches execution failures across active parent workflows via n8n Error Triggers.
  * Logs failure timestamps, node names, workflow titles, and error messages directly into **Google Sheets**.
  * Dispatches instant alerts to designated **Slack** channels.

---

## ⚙️ Tech Stack & Integrations

* **Orchestration:** n8n (with LangChain nodes)
* **AI & LLMs:** OpenAI (`GPT-4o-mini`, `GPT-4o`), Google Gemini (`2.0 Flash`)
* **Vector Database:** Pinecone
* **Communication:** Gmail API, Telegram Bot API, Slack API
* **Storage & Productivity:** Google Drive, Google Sheets

---

## 📥 Setup & Installation

1. **Clone the Repository:**
   ```bash
   git clone [https://github.com/your-username/cogniflow-ai-suite.git](https://github.com/your-username/cogniflow-ai-suite.git)
