# Workflow Analysis for n8n ChatGPT ChatBot

## Description
This workflow powers an AI chatbot designed to assist users on a website. It can engage in conversations, ask for user details like name and email, generate invoices upon request by calling an external workflow, and provide a booking link for appointments.

## Input Details
The workflow is triggered when a new chat message is received, initiating a conversation with the user.

## Process Summary
The workflow begins when a user sends a chat message, activating the "When chat message received" trigger. The "AI Agent" then processes this message, using an OpenAI Chat Model (gpt-4o-mini) to understand and generate responses, while maintaining conversation context with a "Window Buffer Memory". The agent's behavior is guided by a system message that dictates it should first ask for the user's name and email in new conversations. If the user requests an invoice and provides their name and email, the "AI Agent" utilizes the "Invoice Generator" tool to call another n8n workflow, passing the collected user details. If the user wants to book an appointment, the agent directs them to a specific booking URL.

## Output Details
The workflow produces natural language responses delivered back to the user via the chat interface, which may include generated invoice links or direct links for booking appointments.
