# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI, acting as a sales agent to answer questions and capture lead information.

## Input Details
The workflow is triggered by an incoming message to a WhatsApp business account, containing customer inquiries or responses.

## Process Summary
The workflow first extracts the incoming message and phone number. It then retrieves the conversation history (if any) for that contact from a Google Sheet and sends the current message, history, and a predefined system prompt to the OpenAI Chat Completion model to generate a response. The AI processes the query, identifies if a lead has been captured, and updates the Google Sheet with the latest conversation and lead status. Finally, it sends the AI-generated response back to the customer via WhatsApp.

## Output Details
The workflow responds to the customer on WhatsApp with an AI-generated message and updates a Google Sheet with conversation logs and lead information.
