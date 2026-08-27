# 📈 AI-Powered Stock Earnings RAG Workflow

<div align="center">

[![n8n](https://img.shields.io/badge/n8n-Workflow-orange?style=for-the-badge&logo=n8n)](https://n8n.io/)
[![RAG](https://img.shields.io/badge/Architecture-RAG-blue?style=for-the-badge)](https://en.wikipedia.org/wiki/Retrieval-augmented_generation)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT4-red?style=for-the-badge&logo=openai)](https://openai.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

**An intelligent n8n automation that ingests financial reports and utilizes Retrieval-Augmented Generation (RAG) to provide precise financial insights.**

</div>

---

## 📖 Overview

The **Stock Earnings RAG Workflow** is a sophisticated low-code pipeline that automates the analysis of complex financial documents. By leveraging Retrieval-Augmented Generation (RAG) directly within n8n, this system processes dense quarterly earnings reports, creates vector embeddings, and allows users to query the data using natural language.

This project demonstrates advanced knowledge in financial data automation, vector database integration, and LLM-based document querying.

## ✨ Features

- **📂 Document Ingestion Pipeline**: Automatically ingests and chunks large PDF or text-based stock earnings reports.
- **🧠 Intelligent Embedding**: Uses OpenAI's embedding models to convert financial text into highly accurate vector representations.
- **🔍 Retrieval-Augmented Generation (RAG)**: Retrieves the most relevant financial context before passing it to the LLM, effectively eliminating hallucinations.
- **💬 Natural Language Querying**: Allows analysts to ask specific questions like *"What was the YoY revenue growth?"* or *"What are the key risk factors mentioned?"*
- **⚡ Seamless n8n Orchestration**: Entirely visual, low-code architecture that is easily modifiable and highly scalable.

## 🚀 Quick Start

### 1. Prerequisites

- A running instance of [n8n](https://n8n.io/)
- OpenAI API Key
- Access to a Vector Database (e.g., Qdrant, Pinecone, or n8n's built-in memory)

### 2. Installation

1. Clone this repository or download the `workflow.json` file.
2. Open your n8n workspace.
3. Click on **Add Workflow** -> **Import from File** and upload the `workflow.json`.

### 3. Configuration

- **API Keys**: Configure your OpenAI credentials in the relevant nodes.
- **Vector Store Setup**: Ensure the Vector Store node is connected to your preferred database (instructions are included within the workflow notes).
- **File Input**: Point the initial trigger/read node to the directory or cloud storage where your earnings reports are stored.

### 4. Usage

1. **Index Mode**: Run the first part of the workflow to ingest and vectorize the latest earnings report.
2. **Query Mode**: Trigger the Chat node and ask questions about the ingested report to receive highly accurate, cited answers.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to suggest new financial data sources or improvements to the chunking logic.

## 📜 License

This project is licensed under the MIT License.
