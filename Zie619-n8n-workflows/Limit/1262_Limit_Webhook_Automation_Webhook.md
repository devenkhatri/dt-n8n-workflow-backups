# Workflow Analysis for AI Voice Chat using Webhook, Memory Manager, OpenAI, Google Gemini & ElevenLabs

## Description
This workflow enables an AI voice chat experience by processing incoming voice messages, understanding the conversation context, generating a text response using AI, and then converting that response back into audio.

## Input Details
The workflow is triggered by an incoming HTTP POST request to a webhook endpoint, receiving a voice message.

## Process Summary
First, the incoming voice message is transcribed into text using OpenAI's Speech-to-Text service. Next, the workflow retrieves the existing conversation history to maintain context. A Google Gemini chat model then processes the transcribed text along with the conversation history to generate a relevant text response. This response is saved to update the conversation context. Finally, ElevenLabs is used to convert the AI-generated text response back into an audio format.

## Output Details
The workflow sends the generated audio response back to the original webhook caller as a binary response.

## Tags
automation,n8n,production-ready,excellent,optimized
