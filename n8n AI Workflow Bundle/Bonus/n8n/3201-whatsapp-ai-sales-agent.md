# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI to provide product information, answer questions, and handle sales inquiries.

## Input Details
The workflow is triggered by an incoming message from a customer on WhatsApp via a webhook.

## Process Summary
The workflow receives a WhatsApp message and extracts the user ID and message content. It then fetches previous chat history if available, and composes a prompt for the AI with the current message and chat history. The AI generates a tailored response based on the customer's query and the sales agent persona. Finally, the AI's response is sent back to the customer on WhatsApp, maintaining human-like interaction.

## Output Details
The workflow sends an AI-generated response back to the customer on WhatsApp.
