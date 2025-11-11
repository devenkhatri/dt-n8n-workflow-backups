# Workflow Analysis for Research

## Description
This workflow performs AI-powered research by sending a predefined search term to the Perplexity API and retrieving concise, up-to-date information on the topic.

## Input Details
The workflow is manually triggered and uses a preset research term ('Anthropic latest developments') defined within the workflow.

## Process Summary
The workflow starts with a manual trigger. It then sets a predefined research term using a Set node. This term is passed to the Perplexity AI API via an HTTP POST request, which is configured to return a precise and concise response. The API call uses the 'sonar' model and includes the research term in the user message. The response from Perplexity contains the AI-generated research summary.

## Output Details
The workflow outputs the AI-generated research response from the Perplexity API, which can be viewed in the n8n interface or passed to subsequent nodes for further processing.

## Tags
research, AI, Perplexity, API, manual trigger, information retrieval
