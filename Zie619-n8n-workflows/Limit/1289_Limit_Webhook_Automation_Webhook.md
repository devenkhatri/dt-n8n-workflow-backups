# Workflow Analysis for AI Voice Chat using Webhook, Memory Manager, OpenAI, Google Gemini & ElevenLabs

## Description
Automated workflow: AI Voice Chat using Webhook, Memory Manager, OpenAI, Google Gemini & ElevenLabs. This workflow integrates various services to provide an AI voice chat experience, maintaining conversation context.

## Input Details
The workflow is triggered by a webhook receiving a POST request containing a voice message.

## Process Summary
First, the incoming voice message is transcribed into text using OpenAI. Then, existing chat context is retrieved and aggregated. A Basic LLM Chain, powered by Google Gemini, processes the transcribed text along with the conversation history to generate a textual response. This user input and AI response are then saved to maintain context. Finally, ElevenLabs converts the AI's text response into audio.

## Output Details
The workflow produces an audio response from ElevenLabs and sends it back as a binary response to the triggering webhook.

## Tags
automation,n8n,production-ready,excellent,optimized
