# Workflow Analysis for WhatsApp AI Chatbot Integration

## Description
This workflow automates replies to WhatsApp messages using an AI chatbot, stores chat history, and handles media attachments.

## Input Details
The workflow is triggered by an incoming WhatsApp message via a webhook.

## Process Summary
First, the workflow receives an incoming WhatsApp message. It then retrieves the chat history from a Supabase database. The message text and chat history are sent to an OpenAI GPT-3 model to generate a response. The generated AI response is then sent back to the user on WhatsApp. Finally, the interaction, including any media, is stored in the Supabase database.

## Output Details
The workflow sends an AI-generated text response back to the WhatsApp sender and stores the entire conversation, including media, in a Supabase table.
