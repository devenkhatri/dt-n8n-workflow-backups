# Workflow Analysis for Telegram Voice Assistant and Webhook AI Summarizer

## Description
This workflow integrates two distinct AI capabilities: one acting as a voice assistant via Telegram, and another as a research summarization agent triggered by a webhook.

## Input Details
The workflow is triggered by either a voice message sent to a Telegram bot or an HTTP POST request containing a search query to a dedicated webhook.

## Process Summary
When a voice message is received on Telegram, the workflow downloads the audio, transcribes it to text using ElevenLabs, and then uses an AI agent (OpenRouter) to generate a funny text response. This response is converted back to speech by ElevenLabs and sent as an audio file to the user on Telegram. Upon receiving a webhook, the workflow queries a Perplexity AI model with the provided input. An AI agent (OpenRouter) then summarizes the Perplexity response into a concise, three-sentence summary, which is returned as the webhook's response.

## Output Details
The workflow either sends an AI-generated audio response to the Telegram user or provides an AI-summarized text response to the initiating webhook.
