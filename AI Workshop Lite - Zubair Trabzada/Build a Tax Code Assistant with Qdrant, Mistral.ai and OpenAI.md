# Workflow Analysis for AI-Powered Legal Assistant for Texas Tax Codes

## Description
This n8n workflow creates an AI-powered legal assistant that answers questions about Texas tax codes. It downloads official tax code PDFs, processes them to extract structured chapter and section information, and stores this data in a Qdrant vector database using Mistral AI embeddings. The assistant then leverages an AI agent with specialized tools to answer user queries and retrieve specific tax code sections.

## Input Details
The workflow can be triggered manually to ingest and process tax code data or by receiving a chat message as a prompt for the AI assistant.

## Process Summary
1. It downloads and extracts Texas tax code PDFs from a zip file. 2. It extracts text content from each PDF and meticulously parses it into structured chapters, sections, titles, and content. 3. The extracted content is chunked, and embeddings are generated using Mistral AI, which are then stored in a Qdrant vector store with rich metadata. 4. For user interactions, an AI Agent powered by OpenAI Chat Model and conversational memory processes incoming chat messages. 5. The AI Agent utilizes two custom tools: one for querying the Qdrant knowledge base with embeddings to answer questions, and another for searching specific tax code sections by chapter or section number.

## Output Details
The workflow populates a Qdrant vector store with processed Texas tax code data and, when used as a chatbot, provides detailed answers or specific tax code section texts in response to user queries.
