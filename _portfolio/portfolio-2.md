---
title: "End to end RAG pipeline on financial news"
excerpt: " Deployed a streaming pipeline in AWS that converts real-time news to embeddings and store them in a vector database. Takes user queries and extracts relevant context from the vector database and gives answers using LLMs<br/><img src='/images/streaming_pipeline.png'>"
collection: portfolio
---
### Project overview


RAG (Retrieval-Augmented Generation) enhances LLMs' ability to use up-to-date information in text generation. Our project extracts real-time financial news, converts it into embeddings, and stores these in a vector database. During inference, we match user queries with relevant context before generating answers using LLMs.

### Data Ingestion

1. We use Bytewax to efficiently process streaming data from the Alpaca financial news API, converting it into embeddings and storing them in the Qdrant vector database.
2. Our streaming pipeline is containerized and pushed to AWS ECR. We then deploy this container on an EC2 instance to continuously perform the data ingestion process.

### Inference

1. We leverage Mistral 7B model from AWS Bedrock to answer user queries. The model extracts relevant context from our vector database to provide accurate and up-to-date responses.
2. The inference system is deployed as a Fast API, ensuring quick and efficient access for users.

### Flowchart

![Streaming Pipeline](/images/streaming_pipeline.png)


### Tools used 

AWS : ECR, EC2, Bedrock , bytewax, Qdrant vector database and Fast API

#### Next steps

- Perform advanced RAG and analyze the feasibility of knowledge graphs
- Evaluate the performance of this RAG pipeline using RAGAS
- Deploy the inference pipeline in AWS
- Use Terraform to manage infrastructure
- Build a nice front-end system for this application

### Code

Refer to the code[ here](https://github.com/bharathsanthanam94/Real-time-RAG-finance-news)
