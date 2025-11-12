# Workflow Analysis for Tech Radar

## Description
This workflow automates the management and querying of a Tech Radar system that tracks technologies across multiple companies. It transforms data from Google Sheets into both a MySQL database for structured SQL queries and a Google Doc that gets converted into vector embeddings for semantic (RAG) searches. An AI-powered chat interface allows users to ask questions, and an intelligent router decides whether to answer using SQL or RAG based on the nature of the query.

## Input Details
The workflow is triggered either by a scheduled cron job (monthly) for data syncing or by a POST webhook request containing a user's chat question.

## Process Summary
First, the workflow reads technology data from a Google Sheet. It transforms each row into a plain-text paragraph and updates a Google Doc. Separately, when the Doc is updated, it is split into chunks, embedded using Google's text-embedding model, and stored in a Pinecone vector database. On a monthly schedule, the MySQL database is cleared and repopulated from the same Google Sheet. When a user sends a question via webhook, an LLM router determines if the question requires SQL lookup or RAG search, then delegates to the appropriate subworkflow. The final answer is guarded by a prompt that ensures alignment with strategic guidance before being returned.

## Output Details
The workflow outputs a natural language response to the user's question via the webhook response, after routing through either an SQL-based or RAG-based AI agent and applying output guardrails.

## Tags
Tech Radar, RAG, SQL Agent, Google Sheets, MySQL, Pinecone, Vector Database, AI Agent, n8n, Automation, Google Drive, Embeddings, LLM Router, Webhook API
