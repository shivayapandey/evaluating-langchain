### BeyondLLM Integration with LangChain

Welcome to the BeyondLLM integration with LangChain repository! This project demonstrates how to combine the power of BeyondLLM and LangChain to build and evaluate a document retrieval and question-answering system utilizing Retrieval-Augmented Generation (RAG).

### Project Overview

This notebook showcases a step-by-step approach to integrating BeyondLLM with LangChain. By leveraging the capabilities of both tools, we create a system that can effectively retrieve relevant documents based on a query and provide accurate, context-aware answers. The system is further evaluated using BeyondLLM's evaluation metrics, such as Context Relevance, Answer Relevance, and Groundedness.

### Key Features

- **Document Loading and Processing**: Load PDF documents from a directory and split them into manageable chunks for processing.
- **Embeddings Generation**: Create embeddings for the document chunks using pre-trained HuggingFace models.
- **Vector Store**: Store the document chunks in a FAISS vector store for efficient similarity searches.
- **Retriever Setup**: Set up a retriever to find the most relevant documents based on user queries.
- **Language Model Integration**: Integrate LangChain with Groq's Llama-based model to generate answers based on retrieved documents.
- **RAG Chain Creation**: Define a Retrieval-Augmented Generation (RAG) chain that combines document retrieval and language model generation to produce responses.
- **Evaluation Metrics**: Use BeyondLLM to evaluate the generated answers based on context relevance, answer relevance, and groundedness.

### Modules and Libraries Used

- **LangChain**: A framework for building language model-based applications, particularly for document retrieval and question answering.
- **BeyondLLM**: A tool for evaluating language model outputs based on various metrics like context relevance and groundedness.
- **Sentence-Transformers**: For creating embeddings from textual data.
- **ChromaDB**: A fast and scalable database for storing and querying embeddings.
- **Llama-cpp-python**: Integration with Groq's Llama-based models.
- **LangChain Community**: Additional utilities and components for LangChain.
- **pypdf**: A Python library for handling PDF files.
- **FAISS**: A library for efficient similarity search and clustering of dense vectors.
- **PySBD**: A rule-based sentence boundary disambiguation library for tokenizing sentences.

### How It Works

1. **Document Loading**: Load and parse PDF documents from a specified directory using PyPDFDirectoryLoader.
2. **Text Splitting**: Split the loaded documents into smaller chunks using a text splitter to handle large documents effectively.
3. **Embedding Creation**: Generate embeddings for the document chunks using a pre-trained model from HuggingFace.
4. **Vector Store Setup**: Store the embeddings in a FAISS vector store, allowing for fast similarity searches.
5. **Query Processing**: Retrieve the most relevant documents based on a user query using the retriever.
6. **Language Model Invocation**: Pass the query and context to Groq's Llama-based model for generating an answer.
7. **Evaluation**: Evaluate the generated answers using BeyondLLM's evaluation metrics, ensuring that the responses are relevant, grounded, and contextually appropriate.

### Evaluation Metrics

- **Context Relevance**: Measures how well the retrieved documents match the query context.
- **Answer Relevance**: Assesses the accuracy of the generated answer based on the context.
- **Groundedness**: Evaluates how well the generated statements are grounded in the provided context.

### Conclusion

By integrating BeyondLLM with LangChain, this project demonstrates a robust approach to building a document retrieval and question-answering system. The use of advanced evaluation metrics ensures that the generated answers are not only accurate but also contextually relevant and grounded in the provided documents.

Feel free to explore the notebook and adapt the methods for your own use cases!
