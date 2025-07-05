# 🧠 Codex Java - AI-Powered Java Chatbot Assistant

Codex Java is a lightweight, fully functional, **AI-based coding assistant** built using **Python, Flask, LangChain, HuggingFace Embeddings**, and **Pinecone Vector Store**. It helps users with Java programming-related queries by retrieving answers from a custom PDF/document knowledge base.

> Built as a project to demonstrate how to create a local LLM-powered RAG (Retrieval-Augmented Generation) chatbot.

---

## 📸 Demo

[Codex Java Chat UI](C:\Users\Abhishek SHUKLA\OneDrive\Pictures\Screenshots\Screeshot(1)) <!-- Optional: Add screenshot here -->

---

## 🚀 Features

- 🧠 Local LLM support (via `CTransformers`)
- 📚 Ingests custom PDFs and documents (Java tutorials, etc.)
- 🔍 Semantic Search with Pinecone Vector Store
- 💬 Real-time chat interface with Flask
- 📄 Code formatting in responses
- 🔐 Environment variable support via `.env`

---

## 📁 Project Structure

AI_JAVA_CHATBOT/
│
├── app.py # Flask application
├── store_index.py # Loads PDF data and stores embeddings
├── src/
│ ├── helper.py # Embedding, loading, splitting logic
│ └── prompt.py # Prompt templates
│
├── data/ # Folder for PDF files
├── templates/
│ └── chat.html # Chat UI template
├── static/
│ └── style.css # Custom CSS
├── model/ # Local LLaMA or other supported model
├── .env # API keys and environment vars
├── requirements.txt
└── README.md


---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/AI_JAVA_CHATBOT.git
cd AI_JAVA_CHATBOT
```
### 3. Install Dependencies
pip install -r requirements.txt

### 4. Setup .env File
Create a .env file in the root directory:
PINECONE_API_KEY=your_pinecone_key
PINECONE_API_ENV=your_pinecone_environment

Usage

### 1. Embed and Store PDFs in Pinecone
python store_index.py

### 2. Run the Flask App
python app.py

Visit http://localhost:8085 in your browser

🧠 Model Used
Model: LLaMA (or any compatible Hugging Face model)

Loader: CTransformers

Embedding: sentence-transformers/all-MiniLM-L6-v2

You can customize the model path and parameters in app.py.

🙋‍♂️ Author
Made with by Abhishek Shukla

