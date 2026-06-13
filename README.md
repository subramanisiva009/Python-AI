# 🤖 Gemini RAG Assistant

A Retrieval-Augmented Generation (RAG) application built using Streamlit, FAISS, Sentence Transformers, and Google Gemini. This project allows users to upload a DOCX document and interact with it through a chatbot interface. The system retrieves relevant document content and uses Gemini to generate accurate, context-aware responses.

## Features

* Upload DOCX files as a knowledge base
* Semantic search using Sentence Transformers
* Fast vector similarity search with FAISS
* Context-aware response generation using Gemini
* ChatGPT-style chat interface with Streamlit
* Chat history support
* Retrieved context viewer for transparency

## Tech Stack

* Python
* Streamlit
* Google Gemini API
* Sentence Transformers
* FAISS
* NumPy
* Python-Docx
* Python-Dotenv

## Project Workflow

1. Upload a DOCX document.
2. Extract text paragraphs from the document.
3. Generate embeddings using Sentence Transformers.
4. Store embeddings in a FAISS vector index.
5. Convert user questions into embeddings.
6. Retrieve the most relevant document chunks.
7. Send the retrieved context and question to Gemini.
8. Display the generated response in the chat interface.

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/gemini-rag-assistant.git
cd gemini-rag-assistant
```

Install dependencies:

```bash
pip install streamlit python-docx sentence-transformers faiss-cpu numpy python-dotenv google-generativeai
```

## Environment Setup

Create a `.env` file in the project root:

```env
GEMINI_APIKEY=YOUR_GEMINI_API_KEY
```

## Running the Application

```bash
streamlit run app.py
```

The application will open in your browser automatically.

## Folder Structure

```text
project/
│
├── app.py
├── .env
├── requirements.txt
├── README.md
└── sample_documents/
```

## Example Use Cases

* Educational document question answering
* Personal knowledge base assistant
* Research document exploration
* Company policy assistant
* Technical documentation chatbot

## Future Enhancements

* Voice input support
* Voice response generation
* PDF document support
* Multi-document retrieval
* Conversation memory
* Advanced chunking strategies
* Cloud deployment

## Author

Siva Prasad

## License

This project is licensed under the MIT License.
