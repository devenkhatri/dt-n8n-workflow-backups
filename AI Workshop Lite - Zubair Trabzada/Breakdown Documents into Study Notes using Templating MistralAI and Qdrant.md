# Workflow Analysis for AI-Powered Document Processing and Note Generation Workflow

## Description
This workflow automatically processes newly added documents in a specified folder, extracts their content, and uses AI to generate structured study materials like study guides, briefing documents, and timelines based on predefined templates.

## Input Details
The workflow is triggered when a new file is added to the '/home/node/storynotes/context' folder, and it receives the file path and basic file metadata.

## Process Summary
The workflow first imports and extracts text from the new file (supporting PDF, DOCX, and text formats), then creates a summary and stores the document content in a Qdrant vector database with Mistral Cloud embeddings. It then iterates through three document templates (study guide, briefing doc, timeline), using AI agents to generate relevant questions, retrieve context from the vector store, and create comprehensive markdown-formatted documents. Finally, the generated documents are saved to the same folder as the original file with descriptive names.

## Output Details
The workflow produces three AI-generated markdown documents (study guide, briefing document, and timeline) for each input file and saves them to the local filesystem alongside the original document.

## Tags
document processing, AI, note generation, vector store, Mistral AI, Qdrant, study materials, RAG, file automation, text extraction
