# ChatGroq Web Document Q&A with Streamlit 🤖📄

This project is a **Streamlit-based Retrieval-Augmented Generation (RAG) application** that allows users to ask questions about web documentation and receive accurate answers using **Groq LLMs**, **LangChain**, and **FAISS**.

The app loads documentation from a given website, embeds the content, stores it in a vector database, and retrieves relevant context to answer user queries.

---

## 🚀 Features

- Web-based document loading using LangChain
- Text chunking with overlap for better context retrieval
- Vector storage using FAISS
- Fast inference using Groq LLMs
- Interactive Streamlit UI
- Document similarity search with expandable context view

---

## 🧠 How It Works

1. Loads documentation from a web URL
2. Splits documents into manageable chunks
3. Converts text into embeddings
4. Stores embeddings in a FAISS vector store
5. Retrieves relevant chunks based on user query
6. Uses ChatGroq to generate context-aware answers

---

---

## ▶️ How to Run

### 1. Install Dependencies
```bash
pip install streamlit langchain langchain-groq langchain-community faiss-cpu python-dotenv openai
2. Set Environment Variables
Create a .env file:
.env
GROQ_API_KEY=your_groq_api_key_here
OPENAI_API_KEY=your_openai_api_key_here

3. Run the Application
streamlit run app.py

🧪 Usage
Enter a question related to the loaded documentation
Get an answer generated strictly from the retrieved context
Expand Document Similarity Search to view matched document chunks

🛠️ Tech Stack
Python
Streamlit
LangChain
Groq LLM (Mixtral)
FAISS
OpenAI Embeddings

⚠️ Notes
The app loads only the first 50 documents for performance reasons
Designed for learning and experimentation with RAG pipelines
Not intended for production-scale deployments
