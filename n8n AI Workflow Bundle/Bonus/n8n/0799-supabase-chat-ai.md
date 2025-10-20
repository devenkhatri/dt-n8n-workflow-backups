# Workflow Analysis for Supabase Chat AI Workflow

## Description
This workflow processes incoming chat messages, enriches them using AI, stores them in Supabase, and manages chat history for contextual responses.

## Input Details
The workflow is triggered by a webhook, receiving chat messages and user information.

## Process Summary
The workflow starts by extracting user input and user ID. It then checks for existing chat history in Supabase based on the user ID, creating a new one if none exists. The input message is embedded using OpenAI and stored in Supabase with the chat history. The embedded message is then used to query similar past messages from Supabase. Finally, the workflow generates an AI response based on the chat history and new input, which is then returned.

## Output Details
The workflow returns an AI-generated chat response.
