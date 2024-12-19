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


## Setup ⚙️

1. **Mount Google Drive** 💾

   First, mount your Google Drive to access the PDF files or documents you wish to query.

   ```python
   from google.colab import drive
   drive.mount('/content/drive')
   ```

2. **Upload Files** 📥

   Provide the file paths for PDFs or other documents you wish to process.

   ```python
   uploaded_files = input("Enter the paths of your files separated by commas: ").split(',')
   ```

3. **Process Files** 📝

   After specifying the files, you can choose to process them by extracting and chunking the content. The text will be stored in a vector database for later retrieval.

   ```python
   process = input("Process files? (yes/no): ").strip().lower() == 'yes'
   ```

4. **Ask Questions** ❓

   Once the files are processed, interact with the content by asking questions related to the uploaded documents.

   ```python
   user_question = input("Ask a question about your files (or type 'exit' to quit): ").strip()
   ```

   Example:

   ```bash
   Ask Your PDF
   Enter the paths of your files separated by commas: /content/drive/MyDrive/ProjectFolder/Sample2.pdf
   Process files? (yes/no): yes
   Ask a question about your files (or type 'exit' to quit): What is Task 2?
   ```

   The system will retrieve the relevant context and generate an answer based on the information in your files.

## Usage 🛠️

### 1. Mount Google Drive 💾

The notebook allows you to mount Google Drive to access the files (PDFs and other documents) you wish to query against.

```python
from google.colab import drive
drive.mount('/content/drive')
```

### 2. Process Files 📝

After mounting the drive, provide the file paths for PDFs or other documents. You can choose to process multiple files at once.

```python
uploaded_files = input("Enter the paths of your files separated by commas: ").split(',')
process = input("Process files? (yes/no): ").strip().lower() == 'yes'
```

### 3. Ask Questions ❓

Once the files are processed, you can interact with the content by asking questions.

```python
user_question = input("Ask a question about your files (or type 'exit' to quit): ").strip()
```

### 4. Example Interaction 💬

```bash
Ask Your PDF
Enter the paths of your files separated by commas: /content/drive/MyDrive/ProjectFolder/Sample2.pdf
Process files? (yes/no): yes
Ask a question about your files (or type 'exit' to quit): What is Task 2?
```

The model will retrieve relevant information from the files and provide an answer based on the context stored in the vector database.


## Contributing 🤝

Feel free to fork this repository, submit issues, or open pull requests. Contributions are welcome!

## Acknowledgements 🙏

- Thanks to the developers of [LangChain](https://github.com/hwchase17/langchain) for their amazing work on the language model pipeline.
- Thanks to [Hugging Face](https://huggingface.co/) for providing the transformers and embedding models.
- Thanks to the open-source community for contributing to this project.
```

This README is designed to guide users through setting up, using, and interacting with your project. It includes instructions, code snippets, and examples formatted for clarity.
