# Workflow Analysis for AI Chatbot Workflow

## Description
This workflow facilitates an interactive chat experience with an AI model, allowing users to send messages and receive AI-generated responses.

## Input Details
The workflow is triggered by an HTTP POST request to a webhook, receiving a chat prompt from the user in the request body.

## Process Summary
The workflow starts by extracting the user's chat prompt from the incoming webhook data. It then constructs a messages array, including a system message to set the AI's persona and the user's prompt. This array is sent to an OpenAI chat completion model. The AI's response is then extracted, and a static "Thank you for the message!" reply is prepended to the AI text. Finally, formatted messages are appended to the response.

## Output Details
The workflow responds to the initial HTTP POST request with the AI's generated chat response, along with a "Thank you" message.
