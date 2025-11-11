# Workflow Analysis for BambooHR AI-Powered Company Policies and Benefits Chatbot

## Description
An intelligent HR assistant that helps employees find information about company policies, benefits, and contacts by combining document search with real-time employee data from BambooHR.

## Input Details
The workflow is triggered when an employee starts a conversation via a chat interface (webhook), sending their query to the AI assistant.

## Process Summary
First, the workflow loads and indexes company policy documents (PDFs from BambooHR's 'Company Files') into a Supabase vector store for semantic search. When an employee asks a question, the HR AI Agent searches relevant documents and may invoke an employee lookup tool. This tool can retrieve specific employee details by name or identify the most senior person in a department by querying BambooHR's employee database. The AI follows escalation guidelines to provide appropriate contacts when direct information isn't available in policy documents.

## Output Details
The workflow powers a chatbot that responds to employees with answers synthesized from company documents and, when needed, real-time HR data about personnel.

## Tags
HR, chatbot, AI assistant, BambooHR, company policies, employee lookup, vector store, document search, benefits inquiry
