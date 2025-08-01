# 📄 RAG-Powered PDF Q&A Assistant using LlamaIndex & OpenAI

This project demonstrates a Retrieval-Augmented Generation (RAG) system that allows users to ask natural language questions based on the content of PDF documents and receive intelligent, context-aware answers. It integrates **LlamaIndex** for document indexing and retrieval with **OpenAI’s GPT** for response generation, providing a powerful AI-based assistant for document understanding.

---

## 🚀 Features

- 🔍 **Question Answering from PDFs:** Ask any question and receive context-relevant answers based on the document.
- 📚 **Retrieval-Augmented Generation (RAG):** Combines document retrieval with language generation for accurate responses.
- ⚙️ **Modular and Secure Setup:** Uses `.env` for API key management and `requirements.txt` for easy environment replication.
- 📈 **Ideal for Legal, Research, and Enterprise Use Cases.**

---

## 🧠 How It Works

1. **PDF Parsing** – Reads and extracts text from PDFs using `PyPDF`.
2. **Indexing with LlamaIndex** – Text is chunked and converted into vector embeddings.
3. **Query Input** – User provides a natural language question.
4. **Context Retrieval** – Relevant document chunks are retrieved via LlamaIndex.
5. **Answer Generation** – OpenAI’s GPT-4 generates a final response using the retrieved context.

---

## 🛠️ Tech Stack

- **Language:** Python 3.10+
- **Libraries & Tools:**
  - [LlamaIndex](https://github.com/jerryjliu/llama_index)
  - [OpenAI API](https://platform.openai.com/)
  - PyPDF
  - Python-dotenv
  - IPykernel

---

## 📂 Folder Structure

<pre lang="markdown"> ```
  rag-pdf-qa/ 
  ├── main.ipynb # Jupyter Notebook demo for the pipeline 
  ├── requirements.txt # Project dependencies 
  ├── .env # API key file (excluded from version control) 
  ├── README.md # Project documentation ``` </pre>

## 🧪 Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone https://github.com/nithinsankarbahunadam/RAG-Powered-Intelligent-Document-QA-System-.git
   cd rag-pdf-qa
2. **Create and activate a virtual environment:**
   ```bash
   conda create -n ragenv python=3.10
   conda activate ragenv
3. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
4. **Add your OpenAI API Key:**
   Create a file named .env and add the following line:
   ```bash
   OPENAI_API_KEY=your_openai_api_key_here
5. **Launch the Jupyter Notebook:**
   ```bash
   jupyter notebook main.ipynb
