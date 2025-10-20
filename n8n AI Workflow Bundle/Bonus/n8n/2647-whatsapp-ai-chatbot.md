# Workflow Analysis for WhatsApp AI Chatbot

## Description
This workflow enables an AI chatbot on WhatsApp, allowing it to respond to incoming messages automatically using OpenAI.

## Input Details
The workflow is triggered by incoming WhatsApp messages via a webhook.

## Process Summary
The workflow receives a WhatsApp message, extracts the sender's phone number and the message content. It constructs a conversation history and sends it to OpenAI to generate a response. The response from OpenAI is then sent back to the user on WhatsApp.

## Output Details
The workflow sends an AI-generated response back to the original WhatsApp sender.
