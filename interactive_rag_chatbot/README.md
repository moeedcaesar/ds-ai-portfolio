# AI History Chatbot

This project is an **interactive AI-powered chatbot** that answers history-related questions. It leverages **RAG (Retrieval-Augmented Generation)** with PDF documents as knowledge sources, providing factual answers and ending with a short quiz. Built using **Streamlit, LangChain, and Ollama LLMs**.

---

## 🗂️ Project Overview

| Project | Description | Tools |
|---------|-------------|-------|
| AI History Chatbot | Ask history questions and get factually accurate answers with a quiz. Uses a PDF document as context for RAG-based responses. | Python, Streamlit, LangChain, Ollama, Chroma |

---

## 📜 Features

- **Interactive Chat Interface** using Streamlit  
- **Factual Answering** with RAG architecture and PDF context  
- **Memory Management**: Maintains conversation history and can reset with `Exit` command  
- **Off-topic Filtering**: Automatically detects non-history questions  
- **Short Quiz Generation** at the end of each answer  

---

## 🛠️ How It Works

1. **Document Loading:**  
   - PDF document loaded and split into chunks using `RecursiveCharacterTextSplitter`.  
   - Chunks converted to vector embeddings using Ollama embeddings.

2. **RAG Chain:**  
   - Uses **Chroma** vector store for retrieval.  
   - Combines user query, conversation history, and document context to generate answers.

3. **Chatbot Logic:**  
   - Checks if the query is history-related using regex patterns and capitalization heuristics.  
   - Provides factual responses or off-topic warnings.  
   - Clears memory when the user types `Exit`.

4. **Streamlit Frontend:**  
   - Displays chat messages in a user-friendly interface.  
   - Accepts user queries via a chat input.  
   - Dynamically updates the conversation.

---

## ⚡ How to Run

1. Clone the repository:

```bash
git clone <repo_url>
cd ai_history_chatbot
