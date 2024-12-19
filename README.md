# Chat with PDF and Website 📚🌐

This repository provides a Python implementation that allows users to interact with content from PDFs and websites using a **Retrieval-Augmented Generation (RAG)** pipeline. The goal is to extract, process, and embed text from PDFs and websites to answer user queries based on the retrieved content. The system utilizes **LangChain** and **HuggingFace** models to facilitate question answering.

## Overview 🔍

The notebook demonstrates how to:
- 📄 **PDF Processing**: Extracts and processes text from PDFs for querying.
- 🌐 **Website Crawling**: Scrapes and processes website content (to be added).
- 🤖 **Question Answering**: Uses an LLM (Language Learning Model) for generating accurate responses based on the content retrieved.
- 💬 **Conversational Interface**: Interactive chatbot that answers user queries based on the uploaded documents or websites.

### Features 🌟
- **PDF Processing**: Extracts and processes text from PDFs for querying.
- **Website Crawling**: Scrapes and processes website content (to be added).
- **Question Answering**: Uses an LLM (Language Learning Model) for generating accurate responses based on the content retrieved.
- **Conversational Interface**: Interactive chatbot that answers user queries based on the uploaded documents or websites.

## Requirements ⚙️

To run this notebook and the associated scripts, you need to install the following dependencies:

- Python 3.x
- `langchain`
- `PyPDF2`
- `huggingface_hub`
- `sentence_transformers`
- `docx`
- `faiss-cpu` or `faiss-gpu`
- `google.colab` (for Google Colab users)
- `dotenv` (for environment variable management)

You can install the necessary packages using `pip`:

```bash
pip install langchain PyPDF2 huggingface_hub sentence_transformers docx faiss-cpu dotenv


