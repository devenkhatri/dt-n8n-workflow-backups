# Workflow Analysis for AI-Powered Chatbot for BambooHR Policies and Benefits

## Description
This workflow creates an AI-powered chatbot that can answer questions about company policies and benefits using data from BambooHR and a PDF document.

## Input Details
The workflow is triggered by an HTTP request containing a user query about policies or benefits.

## Process Summary
The workflow receives a user query and then fetches relevant employee data from BambooHR, filters for active employees, and retrieves information from a specified PDF file. It then combines the BambooHR data and PDF content to provide context to a large language model (LLM). Finally, the LLM generates a response to the user's query based on the provided context.

## Output Details
The workflow outputs the AI-generated answer to the user's query as an HTTP response.
