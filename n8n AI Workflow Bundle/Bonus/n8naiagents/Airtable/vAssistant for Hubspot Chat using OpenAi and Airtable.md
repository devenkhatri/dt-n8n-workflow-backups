# Workflow Analysis for OpenAI Assistant for HubSpot Chat

## Description
This workflow connects HubSpot chat conversations with an OpenAI assistant, enabling automated, AI-powered responses. It handles new conversations by creating new OpenAI threads and existing ones by continuing the dialogue, and can leverage external tools to gather additional information.

## Input Details
The workflow is triggered by a POST request to a webhook containing details of a new message within a HubSpot chat conversation.

## Process Summary
The workflow retrieves the full HubSpot message, then checks an Airtable database to see if an OpenAI conversation thread already exists for that HubSpot chat. If it's a new conversation, it creates a new OpenAI thread with the message and saves the thread ID to Airtable before initiating an OpenAI assistant run. For ongoing conversations, it adds the new message to the existing OpenAI thread and runs the assistant. If the assistant needs external data, the workflow makes an API call to 'listafirme.ro' to fetch company details, then submits this data back to the assistant. The workflow then polls the assistant's status until it completes, or if it's in progress, it waits and retries.

## Output Details
The workflow posts the final, AI-generated response from the OpenAI assistant back into the original HubSpot chat conversation.
