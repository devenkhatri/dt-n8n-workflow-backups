# Workflow Analysis for WhatsApp AI Lead Responder

## Description
This workflow automates the process of responding to incoming WhatsApp messages using AI. It analyzes the message content, generates a personalized reply, identifies high-value leads, and logs all interactions for record-keeping and follow-up.

## Input Details
The workflow is triggered by an incoming POST request to a "whatsapp-webhook" endpoint, receiving WhatsApp message data including the sender's number and message content.

## Process Summary
1. The workflow is initiated by an incoming WhatsApp message received through a webhook.
2. Key information like the message and sender's number are extracted from the incoming data.
3. An AI model then analyzes the message to determine its intent, sentiment, lead score, and provides a suggested response.
4. A dynamic and personalized reply is crafted based on the AI's analysis, with additional context added for inquiries or support messages.
5. This tailored response is sent back to the original WhatsApp sender, while simultaneously checking if the lead score is high.
6. If the lead score is 7 or above, a dedicated notification is sent to the sales team via WhatsApp to alert them of a high-value lead.
7. All details of the interaction, including the original message, AI analysis, and the AI's response, are appended to a Google Sheet for logging.

## Output Details
The workflow sends an AI-generated WhatsApp reply to the original sender, potentially sends a high-value lead alert to a sales team, and logs all interaction data into a Google Sheet.
