# Workflow Analysis for RAG Workflow For Stock Earnings Report Analysis

## Description
This workflow automatically analyzes the last three quarterly earnings reports for a company (like Google) using Retrieval-Augmented Generation (RAG). It retrieves financial data from PDFs stored in Google Drive, processes and stores them in a vector database, and then uses an AI agent to generate a detailed markdown report with trends, comparisons, and insights, which is saved to Google Docs.

## Input Details
The workflow is triggered manually and receives a list of Google Drive file URLs pointing to earnings report PDFs from a Google Sheet.

## Process Summary
The workflow starts by reading a Google Sheet that lists URLs to quarterly earnings PDFs stored in Google Drive. It downloads each PDF, splits the text into manageable chunks, and generates embeddings using Google Gemini. These embeddings are stored in a Pinecone vector database. When triggered, an AI agent uses the vector store to retrieve relevant financial data from the last three quarters and synthesizes it into a comprehensive markdown report. The final report is saved to a specified Google Doc.

## Output Details
The workflow produces a detailed markdown-formatted financial analysis report and saves it to a Google Doc.

## Tags
RAG, financial analysis, earnings report, AI agent, Pinecone, Google Gemini, Google Drive, Google Sheets, Google Docs, vector database, embeddings, automation, n8n, production-ready
