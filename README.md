# Retrieval-Augmented-Generation

Retrieval-Augmented-Generation built using open-ai gpt-4.
Using: 
1) Langchain for integration
2) Milvus DB for storing embeddings of the documents 

Documents are tokenised and then embeddings are generated using open-ai model which are then stored in the vector database.
While querying, the query string is first converted to embeddings and then the Top-K results are retrieved by searching the query vector using a similartity search 
like the cosine similarity search. 
Then the result is passed as a context in the prompt to the llm. 
Using the RAG method, the llm can answer queries even on data that it has not been trained on.

RAG is a very powerful method to use the LLM to answer queries based on custom data.
