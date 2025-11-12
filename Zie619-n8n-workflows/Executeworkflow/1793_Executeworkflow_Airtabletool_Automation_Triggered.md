# Workflow Analysis for 🤖Contact Agent

## Description
This workflow acts as an AI-powered contact management assistant that can look up, add, or update contact information in an Airtable database based on natural language queries.

## Input Details
The workflow is triggered by another workflow and receives a natural language query in the 'query' field of the input data.

## Process Summary
The workflow starts by receiving a natural language query from another workflow. It uses an AI chat model (GPT-4o) with a system prompt that defines its role as a contact management assistant. Based on the query, it either searches for existing contacts in Airtable or adds/updates a contact using name, email, and phone number extracted by the AI. If successful, it returns the AI's output; if an error occurs during execution, it returns a generic error message.

## Output Details
The workflow outputs either the AI-generated response (on success) or an error message (on failure) in a field named 'response'.

## Tags
contact management, AI assistant, Airtable integration, GPT-4o, workflow automation, data upsert, error handling
