# Workflow Analysis for Google Drive MCP Server for AI-Powered File Reading

## Description
This workflow enables AI agents or MCP clients to securely search for and read the contents of files stored in Google Drive by converting various file formats (PDF, CSV, images, audio, video) into text-based responses that AI systems can understand.

## Input Details
The workflow is triggered either by an MCP server webhook or by another workflow, receiving inputs such as operation type, folderId, and fileId.

## Process Summary
The workflow first checks if the requested operation is 'readFile'. If so, it downloads the specified file from Google Drive. It then inspects the file's MIME type and routes it through the appropriate processing path: PDFs are text-extracted, CSVs are parsed into a string format, images are analyzed using OpenAI's vision model, and audio/video files are transcribed using OpenAI's speech-to-text capabilities. Finally, the extracted or transcribed text is formatted as a response.

## Output Details
The workflow outputs a text-based representation of the requested file's content, which is returned to the calling MCP client or parent workflow for use by AI agents.

## Tags
Google Drive, MCP server, AI integration, file processing, PDF extraction, CSV parsing, image analysis, audio transcription, OpenAI, n8n automation
