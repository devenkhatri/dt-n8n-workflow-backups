# Workflow Analysis for AI Telegram Bot with Supabase Memory

## Description
This workflow creates an AI Telegram bot that maintains conversation context and user memory by integrating with a Supabase database. It allows the bot to provide a more engaging and human-like experience by referencing past interactions with users.

## Input Details
The workflow is triggered by new messages received from a Telegram bot.

## Process Summary
When a new message arrives from Telegram, the workflow first checks if the user exists in a Supabase database. If it's a new user, an OpenAI conversation thread is created, and the user's Telegram ID and OpenAI thread ID are stored in Supabase. The user's message is then sent to the corresponding OpenAI thread, and an AI assistant is run to generate a response. Finally, the generated AI response is retrieved from OpenAI.

## Output Details
The workflow sends the AI assistant's generated response back to the user via Telegram and stores user conversation metadata in Supabase.

## Tags
Telegram, OpenAI, Supabase, Chatbot, AI, Automation, Memory, Contextual, Conversation
