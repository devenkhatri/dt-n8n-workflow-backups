# Workflow Analysis for AI Agent with Custom Activity Suggestion Tool

## Description
This workflow powers an AI chat agent that can suggest personalized activity ideas by calling a custom sub-workflow. When a user asks for something to do—especially when they're feeling bored or want to learn something new—the AI analyzes the request, determines the type of activity and number of participants, then calls the Bored API to fetch a relevant suggestion, which it returns to the user in chat.

## Input Details
The workflow is triggered by a chat message received via the 'When chat message received' node, which passes the user's message as input.

## Process Summary
The main AI agent receives a chat message and uses an OpenAI model with memory to process the conversation. If the user asks for activity suggestions, the agent calls a sub-workflow (used as a custom tool) that extracts the desired activity type and participant count from the input. This sub-workflow then queries the Bored API with those parameters, processes the response, and returns the suggested activity. The main agent receives this result and sends it back to the user in the chat.

## Output Details
The workflow outputs a personalized activity suggestion to the user via the chat interface.

## Tags
AI agent, chatbot, Bored API, custom tool, sub-workflow, OpenAI, activity suggestion, automation, n8n
