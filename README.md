# Multimodal RAG System for PDF Documents

A Streamlit-based application that processes PDF files to extract text, tables, and images; summarizes the extracted data; and uses a retrieval-augmented generation (RAG) pipeline to answer user questions based on the document content. This project leverages multiple APIs and libraries such as OpenAI, Groq, LangChain, and unstructured to provide a multimodal interface for document understanding.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
  - [Running the Web App](#running-the-web-app)
  - [Command-line Execution](#command-line-execution)
- [Configuration](#configuration)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Overview

The **Multimodal RAG System for PDF Documents** is designed to:
- **Extract** content from PDFs, including text, tables, and images using the `unstructured` library.
- **Summarize** the extracted content using custom pipelines that integrate with ChatGroq and ChatOpenAI.
- **Index** the data in a vector store to support efficient retrieval.
- **Answer** user questions by generating context-based responses using a retrieval-augmented generation (RAG) pipeline.

This solution is ideal for scenarios where understanding and querying complex PDF documents in a multimodal format is required.

## Features

- **PDF Upload & Preview:** Upload and view PDF files directly in a Streamlit interface.
- **Content Extraction:** Extracts text, tables, and images from PDFs.
- **Summarization:** Summarizes both textual and visual content for efficient retrieval.
- **Vector Store Integration:** Indexes extracted content to support quick and context-aware retrieval.
- **Retrieval-Augmented Generation:** Uses a RAG pipeline to generate answers based on the retrieved context.
- **API Key Configuration:** Easily integrate your OpenAI, Groq, and LangChain API keys via a configuration file or environment variables.

## Project Structure

├── app.py # Streamlit app for PDF upload, preview, and Q&A 

├── config.py # Configuration for API keys and file paths 

├── extract_data.py # Functions for extracting text, tables, and images from PDFs 

├── main.py # Command-line script to process a PDF and run the RAG pipeline 

├── rag_pipeline.py # Builds the RAG pipeline to generate answers from retrieved context 

├── summarise.py # Contains summarization pipelines for text, tables, and images

├── utils.py # Utility functions (e.g., for image display and document parsing) 

└── requirements.txt # Python dependencies (create this file based on your project needs)
