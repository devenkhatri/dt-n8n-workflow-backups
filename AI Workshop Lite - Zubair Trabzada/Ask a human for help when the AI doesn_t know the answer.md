# Workflow Analysis for AI Human Handoff for Unanswered Queries

## Description
This workflow automates the process of escalating customer queries to a human agent when an AI chat assistant is unable to provide a satisfactory answer, ensuring that no customer question goes unresolved.

## Input Details
The workflow is triggered by an HTTP request containing customer query and potentially chat history information.

## Process Summary
The workflow starts by receiving a customer query and initial chat context via a webhook. It then uses an AI model to attempt to answer the question, creating a dynamic prompt for the AI based on the received input. A "Switch" node checks if the AI's response indicates an inability to answer the query (e.g., "Not enough information", "I am just an AI"). If the AI cannot answer, the workflow assigns a human agent based on current workload and posts the query to a Slack channel for the human agent. The human agent then interacts with the customer through a fresh live chat session via a provided link.

## Output Details
The workflow either returns an AI-generated answer directly to the customer or initiates a human handoff by posting the query to Slack and returning a live chat link for the customer.
