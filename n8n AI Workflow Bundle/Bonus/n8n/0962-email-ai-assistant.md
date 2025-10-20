# Workflow Analysis for AI-Powered Email Assistant

## Description
This workflow acts as an AI assistant for managing emails, allowing users to select an action for incoming emails (reply, summarize, or generate follow-up) and then executes that action using AI models.

## Input Details
The workflow is triggered manually by an HTTP request containing an email subject and body, along with a chosen action.

## Process Summary
The workflow starts by receiving email content and a desired action. It then uses a switch node to determine if the action is to reply, summarize, or generate a follow-up. Based on the chosen action, it constructs a prompt for an AI model (OpenAI GPT-3.5 Turbo or GPT-4), submits the prompt to the AI, and processes the AI's response.

## Output Details
The workflow outputs the AI-generated reply, summary, or follow-up text as an HTTP response.
