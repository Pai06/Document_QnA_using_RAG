# Document Q&A System

This project utilizes the Langchain framework and OpenAI's GPT-3.5 Turbo model to create a document question-and-answer (Q&A) system. It processes PDF documents, allowing users to ask questions and receive relevant answers based on the content.

## Features

- **Document Loading**: Loads and preprocesses PDF documents using `UnstructuredFileLoader`.
- **Text Chunking**: Splits text into manageable chunks with `CharacterTextSplitter` for efficient processing.
- **Vector Embeddings**: Converts text chunks into vector embeddings using `HuggingFaceEmbeddings`.
- **Retrieval-based Q&A**: Retrieves answers to user queries based on document content with `RetrievalQA`.

## Requirements

- Python 3.7 or higher
- OpenAI API key
- Required Python packages:
  - `langchain`
  - `langchain-openai`
  - `langchain-community`
  - `python-dotenv` (for loading environment variables)
  - `huggingface_hub` (if using HuggingFace embeddings)

You can install the required packages using pip:

```bash
pip install langchain langchain-openai langchain-community python-dotenv huggingface_hub
