# PDF Table Data Extraction, Embedding, FAISS Vector Database, and LLaMA 3.1-based Retrieval QA

This repository demonstrates how to:

1. **Extract table data** from PDFs using the `pdfplumber` Python package.
2. **Generate sentence embeddings** for the extracted data using Hugging Face's Sentence Transformers.
3. **Store and search** the embeddings using **FAISS** for efficient similarity searches.
4. **Leverage LLaMA 3.1** for retrieval-based question answering using the retrieved embeddings.

---

## Prerequisites

To run this project, you'll need:

- Python 3.7 or above
- Google Colab or a local environment
- Basic understanding of **Natural Language Processing (NLP)**, **embeddings**, **vector databases**, and **retrieval-based question answering**

---

## Installation

Install the required dependencies using `pip`. In your terminal or Jupyter notebook, run:

```bash
# Install the library for extracting data from PDFs
pip install pdfplumber

# Install FAISS for efficient similarity search
pip install faiss-cpu  # Use faiss-gpu for GPU support

# Install Sentence Transformers to generate text embeddings
pip install sentence-transformers

# Install LangChain for easier handling of documents and embeddings
pip install langchain

# Install Hugging Face Hub for managing the model
pip install huggingface_hub

# Install LLaMA 3.1 for retrieval-based QA (Assuming you've set up Ollama)
pip install ollama

Note:
- use this to run fiass server in local
curl-fsSL https://ollama.com/install.sh | sh
ollama serve & pull llama3.1
