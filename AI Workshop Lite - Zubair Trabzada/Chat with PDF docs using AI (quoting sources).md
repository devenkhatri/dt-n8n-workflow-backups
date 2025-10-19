# Workflow Analysis for Chat with PDF Documents using AI and Source Quoting

## Description
This workflow enables users to interact with PDF documents through an AI chatbot, which provides answers and quotes specific sources from the document.

## Input Details
The workflow is triggered by an HTTP request, receiving user queries and optionally a chat history.

## Process Summary
The workflow first checks for existing chat history. Then, it uses a custom tool to query an AI model (likely a large language model with Retrieval Augmented Generation capabilities) based on the user's input and the content of specified PDF documents. It formats the AI's response, extracting both the answer and the quoted sources from the PDF. Finally, it constructs a comprehensive response including the answer and a list of cited sources.

## Output Details
The workflow outputs an HTTP response containing the AI-generated answer and a list of sources quoted from the PDF document.
