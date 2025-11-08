# Workflow Analysis for Chatbot with Lead Data Enrichment and External Tools

## Description
This workflow powers a chatbot that can process user queries, enriching the conversation with lead data if available, and leveraging external APIs and databases to provide comprehensive responses.

## Input Details
The workflow is triggered by a chat message via a webhook, receiving the user's `chatInput`, a `session_id`, and optionally detailed `leadData`.

## Process Summary
1. Upon receiving a chat message, the workflow first checks if `leadData` (containing user details like name, age, profession, etc.) is provided.
2. If `leadData` is present, it's used to construct a detailed introductory message. This message is then processed by an initial OpenAI assistant ("Chat IA"), which saves this comprehensive lead information into a shared Postgres chat memory for the session.
3. Regardless of whether `leadData` was initially present, the original user's `chatInput` is then passed to a second, main OpenAI assistant ("PINE").
4. The "PINE" assistant utilizes the shared Postgres chat memory (which now includes any enriched lead data) and has access to three external tools: an API for finding information by name and birthdate, a knowledge base for shop information and prices, and a MySQL database for searching product details based on lead criteria.
5. The assistant processes the user's query using this context and these tools to formulate a response.

## Output Details
The workflow generates an AI-powered response based on the user's query and relevant external data, which is returned to the chat interface.
