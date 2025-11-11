# Workflow Analysis for Pitch Deck Analysis and AI Chatbot Workflow

## Description
This workflow automatically processes pitch deck PDFs from Airtable, converts them into markdown using AI vision, extracts key startup information, updates the Airtable record with a detailed report, and builds a searchable vector database to power an AI chatbot that can answer questions about any pitch deck.

## Input Details
The workflow is triggered either manually or automatically when a new pitch deck PDF is uploaded to a specific Airtable base, with required fields like Name and File populated.

## Process Summary
First, the workflow fetches pending pitch decks from Airtable that lack an executive summary. It downloads the PDF, converts each page into separate JPG images using a PDF-to-image service, and unzips the resulting file. The images are resized and sent to a multimodal AI (like GPT-4o) to transcribe each page into structured markdown. All pages are combined, and another AI model extracts structured startup data (like funding stage, founders, traction) based on a VC persona prompt. This extracted data updates the original Airtable record. Simultaneously, the markdown pages are chunked, embedded, and stored in a Qdrant vector database for semantic search, enabling an AI chatbot to answer questions about specific pitch decks.

## Output Details
The workflow updates the Airtable record with extracted startup data and creates a vector store in Qdrant that powers an AI chatbot capable of answering questions about the pitch decks.

## Tags
pitch deck analysis, AI vision, document processing, Airtable integration, vector store, Qdrant, OpenAI, information extraction, RAG, AI chatbot, startup evaluation, PDF to markdown
