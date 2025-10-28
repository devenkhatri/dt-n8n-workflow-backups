# Workflow Analysis for GitHub API Documentation Chatbot with RAG (Pinecone + OpenAI)

## Description
This workflow builds a Retrieval‑Augmented Generation (RAG) chatbot that can answer questions about the GitHub REST API. It first loads the OpenAPI specification from GitHub, splits it into manageable chunks, creates OpenAI embeddings for each chunk, and stores them in a Pinecone vector index. When a user sends a chat message, the workflow embeds the query, searches the Pinecone index for relevant spec fragments, and uses an OpenAI GPT‑4o‑mini model to generate a concise answer that is returned to the user.

## Input Details
The workflow is triggered either by manually clicking “Test workflow” to load the spec, or by receiving a chat message via the LangChain chat webhook, which supplies the user query.

## Process Summary
1. A manual trigger fetches the GitHub OpenAPI JSON via HTTP and sends it to a Pinecone vector store after chunking and embedding with OpenAI. 2. When a chat message arrives, the AI Agent (with a system prompt about the GitHub API) creates an embedding of the query. 3. The Vector Store Tool queries the Pinecone index using this embedding and retrieves the most relevant specification chunks. 4. The retrieved documents are passed to an OpenAI GPT‑4o‑mini model to craft a response. 5. The generated answer is sent back through the chat webhook.

## Output Details
The spec chunks are persisted in the Pinecone index for future retrieval, and each chat query results in a generated answer returned to the user via the webhook response.
