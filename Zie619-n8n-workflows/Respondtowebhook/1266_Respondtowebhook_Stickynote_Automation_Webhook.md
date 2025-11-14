# Workflow Analysis for InstaTest

## Description
This workflow acts as an Instagram chatbot, receiving messages via ManyChat, generating AI-powered responses using ChatGPT, and sending them back to Instagram through ManyChat.

## Input Details
The workflow is triggered by an HTTP POST webhook, receiving message data including session ID and chat text from Instagram via ManyChat.

## Process Summary
First, the workflow receives a message from Instagram via ManyChat. It then sets a system prompt for the AI, defining the persona as an Instagram influencer. An AI agent, utilizing a ChatGPT model and local memory for chat history, generates a simple answer based on the incoming message and the defined prompt. Finally, the generated AI response is sent back.

## Output Details
The workflow produces an AI-generated text response that is sent back via the webhook to ManyChat, which then delivers it to Instagram.

## Tags
automation, n8n, production-ready, excellent, optimized, Instagram, chatbot, AI, ManyChat
