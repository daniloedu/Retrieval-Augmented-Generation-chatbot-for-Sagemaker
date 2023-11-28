# Retrieval-Augmented-Generation-chatbot-for-Sagemaker
The code allows the create a Retrieval-Augmented Generation (RAG) chatbot using open-source tools and AWS services, such as LangChain, Hugging Face, FAISS, Amazon SageMaker, and Amazon TextTract.

Utilizing Amazon SageMaker, AWS services, and various machine learning tools, this project demonstrates how to extract, enrich, and use text data from PDF files to power a context-aware chatbot.

Julien Simon originally created this code from HugginFace and we're using this code only for experimentation purposes.

## Key Components
- **PDF Processing:** Extraction of text from PDFs in the Energy domain using Amazon TextTract.
- **Text Processing:**  Breaking down extracted text into smaller segments for manageability.
- **Feature Extraction:** Enhancing text segments with Hugging Face's feature extraction model.
- **FAISS Indexing:** Storing enriched text in a FAISS index for efficient retrieval.
- **LangChain:** Orchestrating the workflow, from extraction to querying.
- **Large Language Model (LLM):** Querying a Mistral LLM deployed on Amazon SageMaker, incorporating context from the FAISS index.

## Resources 
[LangChain Documentation](https://www.langchain.com/)
[FAISS GitHub](https://github.com/facebookresearch/faiss)
[Embedding Leaderboard](https://huggingface.co/spaces/mteb/leaderboard)
[Embedding Model](https://huggingface.co/BAAI/bge-small-en-v1.5)
[LLM - Mistralai](https://huggingface.co/mistralai/Mistral-7B-Instruct-v0.1)
