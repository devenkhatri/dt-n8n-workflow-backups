# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It leverages OpenAI to understand and respond to customer queries, translates messages for multilingual support, and logs interactions to a Google Sheet for record-keeping and analysis.

## Input Details
The workflow is triggered by an incoming message to a WhatsApp business account.

## Process Summary
The workflow starts by extracting the incoming WhatsApp message. It then translates the message to English using an AI translation service. The translated message is then processed by an AI chat model (OpenAI) to generate a relevant sales response. If needed, the AI response is translated back to the customer's original language. Finally, the original message, AI response, and other relevant details are recorded in a Google Sheet.

## Output Details
The workflow sends an automated AI-generated response back to the customer via WhatsApp and logs the conversation details into a Google Sheet.
