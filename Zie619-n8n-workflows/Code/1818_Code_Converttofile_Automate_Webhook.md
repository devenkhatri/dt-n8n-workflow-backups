# Workflow Analysis for Document Analysis and Chatbot Workflow

## Description
This workflow automatically processes documents submitted via a web form, extracts and analyzes their content using AI, stores the results in a vector database for future reference, and sends a detailed analysis report via email. It also includes a chatbot interface that allows users to ask follow-up questions about the analyzed documents.

## Input Details
The workflow is triggered by a form submission containing one or more files and the user's email address.

## Process Summary
First, the submitted files are split into individual binary items. Each file is sent to a document parsing API, and the system periodically checks the parsing status until it succeeds. The parsed content (in markdown format) is aggregated, translated if needed, and deeply analyzed by an AI agent. The final analysis is converted to a formatted text file, stored in a Pinecone vector database with embeddings, and emailed to the user. A separate chatbot subflow enables interactive Q&A using the stored document data.

## Output Details
The workflow emails a text file containing the AI-generated document analysis to the user and stores the processed content in a Pinecone vector database to power a follow-up chatbot.

## Tags
document processing, AI analysis, file parsing, vector database, chatbot, email automation, form submission, Google Gemini, Pinecone, translation
