# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It receives messages, processes them with AI, and responds intelligently.

## Input Details
This workflow is triggered by an incoming message to a specified WhatsApp number, acting as sales agent.

## Process Summary
Upon receiving a WhatsApp message, the workflow extracts the message content, name and phone number. It then uses an AI model (OpenAI GPT-3.5-turbo-16k) to generate a response based on the message and a predefined system prompt. The generated AI response is then sent back to the customer via WhatsApp.

## Output Details
The workflow sends AI-generated text responses back to the customer on WhatsApp.
