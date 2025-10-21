# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It retrieves customer conversations, processes them with an AI model, and responds via WhatsApp.

## Input Details
The workflow is triggered by an HTTP request containing WhatsApp message data, including a unique ID for the message, the sender's phone number, and the message content.

## Process Summary
The workflow starts by extracting WhatsApp message details from the incoming request. It then retrieves previous messages from the same customer using a Supabase database. An AI model then processes the conversation history and generates a response. Finally, the generated AI response is sent back to the customer via WhatsApp, and the conversation is updated in the Supabase database.

## Output Details
The workflow sends an AI-generated chat response to the customer via WhatsApp and updates the conversation history in Supabase.
