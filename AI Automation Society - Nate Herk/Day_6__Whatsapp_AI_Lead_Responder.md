# Workflow Analysis for WhatsApp AI Lead Responder

## Description
This workflow automates lead qualification and follow-up via WhatsApp using AI to respond to inquiries.

## Input Details
The workflow is triggered by an incoming message to a specified WhatsApp number, acting as a webhook.

## Process Summary
Upon receiving a WhatsApp message, the workflow identifies the sender's phone number. It then checks if the contact already exists in a CRM system. If not, a new contact is created. Subsequently, the message content is sent to an AI assistant (like OpenAI GPT) which generates a response based on the conversation history. Finally, the AI-generated response is sent back to the user via WhatsApp.

## Output Details
The workflow sends AI-generated responses back to the WhatsApp user and updates or creates contact information in a CRM.
