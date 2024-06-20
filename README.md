# PDF Answering Bot

## Overview

This repository contains the code and documentation for developing a Question and Answer (Q&A) bot using the Llama model. The bot is designed to process and comprehend large volumes of text from PDF documents and generate relevant answers to user queries. The project leverages the Langchain framework for document retrieval and FAISS for efficient embedding generation.

## Table of Contents
- [Introduction](#introduction)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Approach](#approach)
- [Failed Approaches](#failed-approaches)
- [Results](#results)
- [Discussion](#discussion)
- [Conclusion](#conclusion)
- [References](#references)

## Introduction

### Problem Statement
The project aims to develop an automated system that can provide accurate and efficient responses to user queries by understanding and processing large volumes of text from PDF documents.

### Objectives
- Develop a Q&A bot using the Llama model.
- Integrate the bot with document retrieval and embedding generation frameworks.
- Evaluate the bot's performance using standard metrics.

## Setup and Installation

### Prerequisites
- Python 3.7+
- pip (Python package installer)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/pdf-answering-bot.git
   cd pdf-answering-bot
2)pip install -r requirements.txt

## Usage
### Load Documents:
Place your PDF documents in the directory and ensure they are processed into text format, loaded through the `input.txt` file. The loader will read this file to process.

### Run the Notebook:
Open and run the Jupyter notebook `pdf_answering_bot.ipynb`. This will execute all the steps to create and evaluate the Q&A bot.

### Ask Questions:
Use the setup Q&A chain to ask questions and receive answers based on the provided documents.

## Approach:

### Methodology:
1. **Environment Setup:** Install necessary libraries and set up the environment.
2. **Configuration:** Set API tokens and model configurations.
3. **Data Loading:** Load documents using `TextLoader`.
4. **Text Splitting:** Split documents into chunks using `CharacterTextSplitter`.
5. **Embeddings Generation:** Generate embeddings using `HuggingFaceEmbeddings`.
6. **Vector Store Creation:** Create a vector store with `FAISS`.
7. **Model Initialization:** Load the Llama model and tokenizer.
8. **Question-Answer Chain Setup:** Establish a question-answering chain.
9. **Performance Evaluation:** Evaluate performance using ROUGE scores.

## Results:

### Performance Metrics:
The performance of the Q&A bot is evaluated using ROUGE scores, which measure the overlap between generated answers and ground truth answers. Detailed metrics and visualizations are provided in the notebook.

## Conclusion:

### Summary of Findings:
The Q&A bot using the Llama model demonstrated good performance in generating relevant answers. Key improvements in text splitting, embedding quality, and vector store efficiency were crucial to the success.

## References:
- HuggingFace Transformers
- FAISS Documentation
- Langchain Documentation
- Rouge Scorer


