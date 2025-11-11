# Workflow Analysis for Voice Workflows

## Description
This workflow processes voice messages from Telegram by converting them to text, generating a humorous AI response, and sending it back as a voice message. It also includes a separate research agent that responds to webhook queries by summarizing information from Perplexity.

## Input Details
The workflow is triggered either by a voice message sent to a Telegram bot or by an HTTP POST request to a webhook endpoint containing a search query.

## Process Summary
When a Telegram voice message is received, the workflow downloads the audio file, transcribes it to text using ElevenLabs, and passes the text to an AI agent powered by OpenRouter with a humorous personality. The AI's text response is converted back to speech using ElevenLabs and sent as an audio reply in Telegram. Separately, when the webhook receives a search query, it fetches relevant information from Perplexity, summarizes it using another AI agent, and returns the summary as a webhook response.

## Output Details
The workflow sends an AI-generated voice message back to the Telegram chat and returns a summarized text response to the webhook caller.

## Tags
telegram, voice, speech-to-text, text-to-speech, AI agent, ElevenLabs, OpenRouter, Perplexity, webhook, conversational AI
