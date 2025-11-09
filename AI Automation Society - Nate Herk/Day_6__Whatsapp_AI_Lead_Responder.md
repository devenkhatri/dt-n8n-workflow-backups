# Workflow Analysis for Day 6- Whatsapp AI Lead Responder

## Description
This workflow automatically responds to incoming WhatsApp messages using an AI assistant that analyzes the message intent, sentiment, and lead potential. It sends a personalized reply, logs the interaction in Google Sheets, and alerts the sales team if the lead is high-value.

## Input Details
The workflow is triggered by a POST request to a WhatsApp webhook containing the sender's phone number and message text.

## Process Summary
When a WhatsApp message is received, the workflow extracts the message and sender info. It sends this data to the DeepSeek AI API to analyze intent, sentiment, and generate a suggested reply along with a lead score. The AI response is parsed, enhanced with contextual follow-up questions, and formatted into a WhatsApp message. The reply is sent back to the customer, and the interaction details are saved to a Google Sheet. If the lead score is 7 or higher, a high-priority alert is sent to the sales team via WhatsApp.

## Output Details
The workflow sends an AI-generated WhatsApp reply to the customer, logs the conversation and analysis in a Google Sheet, and optionally notifies the sales team of high-value leads via WhatsApp.

## Tags
whatsapp, ai, lead scoring, customer support, automation, google sheets, sales notification
