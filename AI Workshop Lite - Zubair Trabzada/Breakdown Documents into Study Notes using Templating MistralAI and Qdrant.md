# Workflow Analysis for AI Document Note Generator

## Description
This workflow automates the generation of various study notes (Study Guide, Timeline, Briefing Document) from newly added source documents. It monitors a local folder for new files, imports their content, summarizes them, and stores their vector embeddings in a Qdrant vector store. Using an AI agent chain powered by Mistral Cloud, it iteratively generates questions about the document, retrieves relevant context from the vector store, and then produces structured markdown documents based on predefined templates. Finally, these AI-generated notes are exported to the filesystem alongside the original source file for easy access and study.

## Input Details
The workflow is triggered when new files (PDF, DOCX, or text) are added to a specified local folder (`/home/node/storynotes/context`), which it then imports for processing.

## Process Summary
1. The workflow detects a new file, extracts its content, and determines its type.
2. The extracted content is summarized using an AI model and then broken into chunks, embedded, and stored in a Qdrant vector database for efficient retrieval.
3. It then iterates through a predefined list of document templates (Study Guide, Timeline, Briefing Doc).
4. For each template, an AI agent generates targeted questions about the document based on its summary, retrieves relevant information from the vector store using these questions, and then generates the complete template document in markdown format.
5. Finally, each generated document is saved as a markdown file in the specified folder.

## Output Details
The workflow produces AI-generated markdown documents (e.g., Study Guides, Timelines, Briefing Docs) and exports them to a local folder, alongside the original source file.
