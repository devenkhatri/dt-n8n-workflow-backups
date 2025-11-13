# Workflow Analysis for AI Telegram Bot with Supabase Memory

## Description
This workflow creates an intelligent Telegram bot powered by OpenAI that can remember users and maintain conversation context across interactions by storing user and conversation data in a Supabase database.

## Input Details
The workflow is triggered by new messages sent to a Telegram bot, receiving the message text and user's Telegram ID.

## Process Summary
When a user sends a message to the Telegram bot, the workflow first checks if the user already exists in the Supabase database. If not, it creates a new OpenAI thread and registers the user with their Telegram ID and the new thread ID. If the user exists, it uses their existing thread. The user's message is sent to OpenAI using the appropriate thread, the assistant processes the message, and the response is retrieved and sent back to the user via Telegram.

## Output Details
The workflow sends AI-generated responses back to the Telegram user and stores user-thread mappings in a Supabase database for persistent conversation memory.

## Tags
telegram, openai, supabase, ai bot, chatbot, conversation memory, automation, n8n
