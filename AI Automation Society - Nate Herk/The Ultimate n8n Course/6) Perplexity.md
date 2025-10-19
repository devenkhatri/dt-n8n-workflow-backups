# Workflow Analysis for Perplexity AI Query Generator

## Description
This workflow demonstrates integration with the Perplexity AI service, specifically designed to execute a predefined query using a powerful online model and a customized system prompt to retrieve a targeted, informational response.

## Input Details
The workflow is started by a Manual Trigger, intended for quick testing or simple execution without requiring external data inputs.

## Process Summary
The workflow is initiated manually. A Set node is used to define the specific user prompt (e.g., a question about n8n features) and to inject a system prompt that defines the AI's expert persona. This structured query and context are then passed to the Perplexity AI node, which generates an informed response using a selected online large language model.

## Output Details
The final output is the generated text response from the Perplexity AI model, ready for subsequent processing, storage, or display.
