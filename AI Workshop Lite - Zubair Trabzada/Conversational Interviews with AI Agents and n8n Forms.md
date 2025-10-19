# Workflow Analysis for Conversational AI Agent Interviewer with n8n Forms

## Description
This workflow facilitates conversational interviews using AI agents and n8n forms. It guides users through an interview process, processes user responses with an AI model, and stores the interaction details.

## Input Details
The workflow is manually triggered or can be initiated via a webhook, receiving information about the user, interview questions, and AI model parameters.

## Process Summary
The workflow starts by retrieving an initial system prompt and user data. It then iteratively asks questions, processes user responses using an AI model to generate follow-up questions or extract information, and logs the conversation.  The AI model determines the next question based on the user's previous answer.

## Output Details
The workflow stores the complete conversation history including questions asked, user answers, and AI responses in an n8n Form component for review.
