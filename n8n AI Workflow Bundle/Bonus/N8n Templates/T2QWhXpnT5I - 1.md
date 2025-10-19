# Workflow Analysis for AI-Powered Real-Time Text Analysis and Response via Webhook

## Description
This workflow automatically processes incoming data from a webhook, uses an advanced AI model (OpenAI) to analyze the text and generate a structured response, cleans the AI output, and then immediately returns the final result via the same webhook. This is suitable for integrating AI analysis into any external system that can send an HTTP request.

## Input Details
The workflow is triggered by an incoming HTTP POST request to a webhook, expecting a JSON payload containing the text or data to be analyzed.

## Process Summary
The workflow starts by receiving a request via webhook. A Function node then prepares a detailed prompt for the AI based on the input data. The OpenAI node processes the prompt and generates a structured text response using a chat completion model. A second Function node is used to clean and extract the useful information from the AI's output, often parsing a JSON string. Finally, a Set node formats the cleaned data before it is returned as an HTTP response to the original caller.

## Output Details
The workflow returns a structured JSON object containing the status and the AI-generated result as an immediate response to the triggering webhook.
