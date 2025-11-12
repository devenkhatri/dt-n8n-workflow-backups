# Workflow Analysis for RAG Workflow For Stock Earnings Report Analysis

## Description
This workflow automatically analyzes the last three quarters of Google's earnings reports using Retrieval-Augmented Generation (RAG). It retrieves financial documents from Google Drive, processes and stores them in a Pinecone vector database, and then uses an AI agent to generate a detailed markdown report highlighting revenue trends, profitability, key metrics, and outliers. The final report is saved to a Google Doc.

## Input Details
The workflow is manually triggered and pulls a list of Google Drive file URLs from a specified Google Sheet that contains links to earnings report PDFs.

## Process Summary
The workflow starts by reading a Google Sheet that lists URLs to Google's quarterly earnings PDFs. It downloads each PDF from Google Drive, splits the text into chunks, generates embeddings using Google Gemini, and stores them in a Pinecone vector database. An AI agent then uses these stored embeddings to retrieve relevant financial data in response to a user query about Google’s last three quarters of earnings. The agent synthesizes this data into a structured markdown report and saves it to a Google Doc.

## Output Details
The workflow produces a formatted markdown financial analysis report and saves it to a specified Google Doc.

## Tags
RAG, financial analysis, earnings report, Google, Pinecone, Google Gemini, AI agent, Google Docs, Google Drive, Google Sheets, vector database, embeddings, n8n, automation, production-ready
