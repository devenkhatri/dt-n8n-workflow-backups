# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp by acting as an AI sales agent, handling queries, qualifying leads, and routing complex issues to human agents.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by retrieving the current date. It then fetches previous conversational memory from a database (Supabase). The AI (OpenAI) processes the incoming message with the conversation history and a predefined persona, then checks for tool calls. If a tool call to handoff to a human agent is detected, it flags the conversation for a human. If not a handoff, it translates the AI response to the user's language (DeepL), stores the updated conversation memory, and sends the AI-generated response back to the user via WhatsApp.

## Output Details
The workflow sends AI-generated conversational responses to the user on WhatsApp and stores conversation history in Supabase, with an option to flag conversations for human intervention.
