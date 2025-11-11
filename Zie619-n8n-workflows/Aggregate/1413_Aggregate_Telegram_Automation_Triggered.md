# Workflow Analysis for DSP Agent - Telegram Study Assistant for Signal Processing

## Description
This workflow acts as an intelligent study assistant for signal processing topics. It receives messages or voice notes from users via Telegram, transcribes voice messages if needed, uses AI to generate helpful, context-aware responses based on the user's query, and replies directly in the Telegram chat. It also stores memory of user interactions in Airtable to personalize future conversations.

## Input Details
The workflow is triggered by incoming Telegram messages or voice notes sent to a Telegram bot.

## Process Summary
The workflow starts by receiving a message or voice note via Telegram. A Switch node checks whether the input is text or voice. If it's text, it proceeds directly; if it's voice, it downloads the file and (intended to) transcribe it using OpenAI. The AI Agent node uses a detailed prompt to generate a helpful educational response based on the input. User memory is retrieved from Airtable and merged with the input to provide context-aware replies. Finally, the AI-generated response is sent back to the user via Telegram.

## Output Details
The workflow sends an AI-generated educational response back to the user in the Telegram chat and optionally stores memory of the interaction in an Airtable base.

## Tags
Telegram, AI Assistant, Signal Processing, Voice Transcription, Educational Bot, Airtable Memory, OpenAI, n8n
