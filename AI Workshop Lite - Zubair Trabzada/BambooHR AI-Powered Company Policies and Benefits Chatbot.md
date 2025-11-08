# Workflow Analysis for BambooHR AI-Powered Company Policies and Benefits Chatbot

## Description
This workflow creates an AI-powered chatbot that assists employees with questions regarding company policies, benefits, and internal contact information by leveraging data from BambooHR and an AI knowledge base.

## Input Details
The workflow is triggered either manually to load company policy files or by an employee initiating a conversation with the chatbot via a chat interface.

## Process Summary
Initially, the workflow retrieves company policy files from BambooHR, filters for PDF documents, splits them into manageable chunks, and stores their embeddings in a Supabase vector database. When an employee asks a question, an AI agent uses this vector store to retrieve relevant policy information. Additionally, the agent can call an employee lookup tool which, based on the query, either searches BambooHR for specific employee details or identifies the most senior person in a requested department, assisting with contact person inquiries and escalation procedures.

## Output Details
The workflow provides conversational responses to employee queries, delivering information on company policies, benefits, and contact details of employees or departmental leaders.
