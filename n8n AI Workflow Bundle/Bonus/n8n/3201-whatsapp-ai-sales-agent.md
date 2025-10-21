# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent to answer queries, overcome objections, and pre-qualify leads before handing them over to a human sales representative.

## Input Details
The workflow is triggered by an incoming message to a WhatsApp business account.

## Process Summary
The workflow starts by extracting the message content and sender information from WhatsApp. It then uses an AI model (OpenAI GPT) to generate a dynamic response based on the customer's query and the predefined sales script. If the AI determines the lead is qualified and ready for a human agent, it sets a flag. Finally, the AI-generated response is sent back to the customer on WhatsApp.

## Output Details
The workflow sends AI-generated sales responses back to the customer on WhatsApp and can potentially flag qualified leads for human intervention.
