# Workflow Analysis for DSP Agent

## Description
A Telegram-based AI assistant designed to help students with digital signal processing (DSP) problems by analyzing text or voice messages, providing guided explanations, and using tools like Wikipedia, calculators, and memory to personalize learning.

## Input Details
The workflow is triggered by incoming messages from Telegram, which can include either text or voice messages.

## Process Summary
The workflow starts by receiving a Telegram message. It uses a Switch node to determine if the message contains text or a voice note. Text is passed directly for processing, while voice messages are downloaded and appear intended for transcription (though transcription is not fully implemented). The system retrieves past user memory from Airtable and merges it with the current message. An AI agent, guided by a detailed system prompt, generates a contextual response using either OpenAI or Google Gemini. The response is sent back to the user via Telegram, and a new memory entry about the user is saved to Airtable for future interactions.

## Output Details
The workflow sends a personalized AI-generated response back to the user via Telegram and stores a summary of the interaction in an Airtable database for memory retention.

## Tags
Telegram, AI Agent, Signal Processing, Voice Message, Text Processing, Airtable, OpenAI, Google Gemini, Educational Assistant, Memory Storage
