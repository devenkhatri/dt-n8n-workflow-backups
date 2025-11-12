# Workflow Analysis for Generate Exam Questions

## Description
This workflow automatically generates both open-ended and multiple-choice exam questions from a Google Doc using AI. It leverages vector databases and large language models to create high-quality, curriculum-aligned assessment questions and stores them in a Google Sheet.

## Input Details
The workflow is manually triggered and receives content from a specified Google Doc via a URL.

## Process Summary
First, the workflow fetches a document from Google Docs and converts it to Markdown. It then creates or refreshes a Qdrant vector collection and stores document embeddings using OpenAI. Next, it generates 10 open-ended and 10 multiple-choice questions using Google Gemini. For open questions, it retrieves accurate answers using a vector database (RAG). For closed questions, it generates one correct and three plausible incorrect answers using RAG. Finally, all questions and answers are written to a Google Sheet.

## Output Details
The workflow outputs exam questions and their answers to specific tabs in a Google Sheet—one tab for open-ended questions with answers, and another for multiple-choice questions with answer options and correct answer indicators.

## Tags
exam generation, AI questions, Google Docs, Google Sheets, Qdrant, vector database, RAG, OpenAI embeddings, Google Gemini, multiple-choice questions, open-ended questions, educational automation, n8n workflow
