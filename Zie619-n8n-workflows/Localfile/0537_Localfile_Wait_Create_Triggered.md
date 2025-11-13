# Workflow Analysis for Local File Triggered Document Generation Workflow

## Description
This workflow automates the process of generating various types of study and briefing documents from newly added source files. It leverages AI models to summarize, analyze, and create structured outputs based on predefined templates.

## Input Details
The workflow is triggered when a new file (PDF, DOCX, or plain text) is added to the /home/node/storynotes/context local directory.

## Process Summary
1. The workflow detects a new file in a specified local folder, imports its content, and identifies its type.
2. It then extracts the text, summarizes it using a Mistral AI model, and stores embeddings of the document in a Qdrant vector database for efficient retrieval.
3. Next, it iterates through a list of predefined document types such as "Study Guide", "Timeline", and "Briefing Doc".
4. For each document type, an AI agent formulates questions based on the document summary and retrieves relevant information from the vector store.
5. Finally, another AI model generates the specific templated document (e.g., Study Guide) by answering the formulated questions using the retrieved information and formats it in markdown.

## Output Details
The workflow exports the AI-generated documents (e.g., Study Guide, Timeline, Briefing Doc) as markdown files to a local folder, with filenames reflecting the generated document type.

## Tags
automation, n8n, production-ready, excellent, optimized
