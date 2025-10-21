# Workflow Analysis for WhatsApp AI Sales Agent with Conversation Memory

## Description
This workflow automates WhatsApp conversations using AI to act as a sales agent, remembering past interactions and continuously training itself based on provided data.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by receiving a WhatsApp message. It then retrieves the conversation history from a Google Sheet and sends the current message and history to a large language model (LLM) for processing, using a prompt that guides its sales agent behavior. The LLM's response is then added to the conversation history in the Google Sheet. Finally, if the LLM generates a valid response, it is sent back as a WhatsApp message.

## Output Details
The workflow sends AI-generated sales responses back to the user on WhatsApp and updates a Google Sheet with the conversation history.
