# Workflow Analysis for Perplexity AI Comparison of n8n and Make

## Description
This workflow leverages Perplexity AI to get a detailed comparison between n8n and Make, providing both the AI-generated answer and relevant citations from specified domains.

## Input Details
The workflow is triggered manually by clicking ‘Test workflow’ and uses predefined parameters for the AI query.

## Process Summary
The workflow starts with a manual trigger. It then sets up system and user prompts for an AI query, along with specific search domains. An HTTP POST request is sent to the Perplexity AI API with these parameters to retrieve information. Finally, the workflow extracts the AI-generated content and any associated citations from the Perplexity AI response.

## Output Details
The workflow outputs the AI-generated answer content and a list of citations obtained from the Perplexity AI service.
