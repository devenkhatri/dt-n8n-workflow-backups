# Workflow Analysis for Automated Document Note Generation Workflow

## Description
This workflow automates the generation of various types of study notes (e.g., study guides, timelines, briefing documents) from source documents. It continuously monitors a local folder for new files, extracts their content, summarizes them, and then uses AI agents to process the information and create templated documents, which are then saved back to the local file system.

## Input Details
The workflow is triggered when a new file is added to the `/home/node/storynotes/context` folder, receiving the file's path and content.

## Process Summary
First, the workflow imports the new document, extracts its text content based on its file type (PDF, DOCX, or plain text), and sets up metadata. Next, it summarizes the document using an AI model and stores the document's content as vector embeddings in a Qdrant vector store for efficient retrieval. The workflow then iterates through predefined document templates (Study Guide, Timeline, Briefing Doc). For each template, an AI agent generates questions based on the document summary, retrieves relevant information from the vector store using these questions, and synthesizes the retrieved information to generate the final templated document. Finally, the generated document is converted to a binary format and exported to a local folder.

## Output Details
The workflow produces markdown-formatted templated documents (e.g., Study Guides, Timelines, Briefing Docs) and saves them to a local folder.

## Tags
automation,n8n,production-ready,excellent,optimized,document processing,AI,LLM,vector store,file system
