# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI, providing instant responses and lead qualification for sales teams.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by extracting the message and sender details from the incoming WhatsApp message. It then uses an AI model (ChatGPT) to generate an appropriate response based on the customer's message, incorporating a predefined sales persona and product information. If the AI determines the message is a lead, it extracts lead information like name, phone, and email using another AI model and stores it in a Google Sheet. Finally, the generated AI response is sent back to the customer on WhatsApp.

## Output Details
The workflow sends automated AI-generated responses back to the WhatsApp sender and optionally logs lead information into a Google Sheet.
