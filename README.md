# 📚 Semantic Book Search using FAISS and Transformers

This is a minor project showcasing how to build a semantic search engine for books using metadata (title + description). It leverages Hugging Face Transformers to generate embeddings and FAISS for efficient similarity search.

## ✨ Features

- Uses `sentence-transformers/multi-qa-mpnet-base-dot-v1` to encode book data into 768-dimensional embeddings.
- Preprocesses and filters a dataset of books with moderate-length descriptions.
- Indexes embeddings with FAISS for fast and scalable vector similarity search.
- Supports querying with natural language to retrieve relevant books semantically.

## 🔧 Tech Stack

- 🤗 Hugging Face Transformers (`sentence-transformers`)
- 🔍 FAISS (Facebook AI Similarity Search)
- 🔥 PyTorch
- 📊 Dataset: Book metadata (title + description)

## 🚀 Steps

1. **Data Filtering**: Books with moderately long descriptions are selected from the dataset.
2. **Text Preparation**: Title and description are merged into a single text field.
3. **Embedding Generation**: Text is encoded using CLS pooling with the `multi-qa-mpnet-base-dot-v1` model.
4. **FAISS Indexing**: The generated embeddings are added to a FAISS index for fast similarity search.
5. **Querying**: A user query is converted into an embedding and matched against the index to find semantically similar books.

## 📝 Fututre Idea

- Use a large scale practical dataset to implement semantic searching using FAISS


Please refer to the notebook for steps and results...
