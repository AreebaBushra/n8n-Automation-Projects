# IntelliSearch – AI Knowledge Assistant

**IntelliSearch** is an AI-powered knowledge retrieval system developed using **n8n**. It integrates **Google Gemini AI**, **Supabase Vector Store**, and **Google Drive** to deliver intelligent, context-aware responses from stored documents. The system leverages **Retrieval-Augmented Generation (RAG)** techniques to enable efficient document-based question answering and knowledge search.

---

## Overview

The IntelliSearch workflow automates document ingestion, embedding generation, vector storage, and intelligent querying. It retrieves relevant content from a connected Google Drive folder, indexes the data in a Supabase vector database, and uses Google Gemini to generate precise, contextually relevant answers based on the retrieved information.

---

## Key Features

* **Automated Document Retrieval:** Fetches and processes documents from a specified Google Drive folder.
* **Semantic Search and Embedding:** Uses Google Gemini embeddings to transform text into searchable vector representations.
* **Context-Aware Query Responses:** Generates intelligent answers using Gemini LLM with document-based context.
* **Persistent Memory:** Maintains conversational history using PostgreSQL for continuity across interactions.
* **End-to-End Automation:** Fully managed within the n8n workflow environment without external coding.

---

## Workflow Components

| Component                       | Function                                                   |
| ------------------------------- | ---------------------------------------------------------- |
| **Webhook Trigger**             | Initiates the workflow when a query is received.           |
| **Google Drive Integration**    | Searches and downloads relevant documents.                 |
| **Data Loader & Text Splitter** | Loads and segments document content for processing.        |
| **Google Gemini Embeddings**    | Converts document text into vector embeddings.             |
| **Supabase Vector Store**       | Stores embeddings for semantic search and retrieval.       |
| **Google Gemini Chat Model**    | Generates responses based on the retrieved context.        |
| **PostgreSQL Memory**           | Stores chat history and session data.                      |
| **LangChain Agent (via n8n)**   | Coordinates query processing, memory, and retrieval tools. |

---

## Technical Stack

* **Platform:** n8n (Workflow Automation)
* **Language Model:** Google Gemini (PaLM API)
* **Database:** Supabase (Vector Storage), PostgreSQL (Chat Memory)
* **Document Source:** Google Drive API
* **Framework:** LangChain for n8n

---

## Workflow Process

1. **Trigger:** A query is sent to the workflow via webhook or manual execution.
2. **Document Retrieval:** Files are searched and downloaded from Google Drive.
3. **Preprocessing:** Documents are loaded and divided into manageable text segments.
4. **Embedding Generation:** Text chunks are embedded using Google Gemini embeddings.
5. **Vector Storage:** Embeddings are indexed in Supabase for retrieval.
6. **Query Handling:** A user’s question is processed and matched with relevant content.
7. **Response Generation:** Gemini LLM generates a contextually grounded response.
8. **Memory Storage:** The conversation is saved in PostgreSQL for future continuity.

---
<img width="864" height="449" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/b2e244f0-7ad2-4021-aa7d-c90b97a87fd5" />
---

## Web Integration

The IntelliSearch workflow is connected to a custom web interface that allows users to send their queries directly through a browser.

### How It Works

The user enters a question on the website.

The web form sends the query to the n8n Webhook Endpoint via a POST request.

The n8n workflow processes the query, retrieves relevant document context, and generates a Gemini-powered response.

The answer is displayed on the website in real time.

Example Flow

Frontend (Website) ➜ Webhook (n8n) ➜ AI Agent ➜ Gemini LLM ➜ Response Returned to User

<img width="1338" height="574" alt="Screenshot 2025-10-20 185703" src="https://github.com/user-attachments/assets/72152957-57ef-4333-a32c-96e9a3a57572" />

---

**Areeba Bushra**
*Data Science & AI Enthusiast | Automation Developer*
📍 Based in Pakistan

