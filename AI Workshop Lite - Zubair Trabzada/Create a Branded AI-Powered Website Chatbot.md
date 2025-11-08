# Workflow Analysis for AI Powered Appointment Booking & Inquiry Chatbot

## Description
This workflow acts as an AI assistant for nocodecreative.io, handling customer inquiries and coordinating appointments. It engages customers, checks calendar availability, books meetings in Outlook, and, if an appointment isn't suitable, forwards detailed customer messages to a human via email.

## Input Details
The workflow is triggered by a chat webhook, receiving customer chat messages as input.

## Process Summary
The workflow receives a chat message and uses an AI agent to process it, leveraging an OpenAI chat model and session memory. The AI agent can perform three main actions: directly create appointments in Microsoft Outlook, check calendar availability by fetching events and calculating free slots, or send detailed customer inquiries as emails. Finally, it responds to the initial chat with the AI's output.

## Output Details
The workflow responds to the initiating chat webhook with the AI agent's conversation output (e.g., availability, appointment confirmation, or further questions), creates calendar events in Microsoft Outlook, or sends an email notification to a predefined recipient with customer inquiry details.
