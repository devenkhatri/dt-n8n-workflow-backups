# Workflow Analysis for Secured AI Content Generator API with API Key Validation

## Description
This workflow exposes a secured API endpoint for on-demand content generation using the OpenAI ChatGPT model (GPT-4 Turbo). It enforces security by requiring and validating a specific API key within the request body before executing the content generation task, ensuring only authorized applications can utilize the AI service.

## Input Details
The workflow is triggered by a POST request to a webhook, expecting a JSON payload that includes the content `query` and an authentication `api_key`.

## Process Summary
The workflow starts with a webhook trigger, splits the input data into single items, and extracts the user's `query` and the provided `api_key`. An IF condition then checks if the submitted `api_key` matches a secure internal key. If the key is valid, the query is passed to the OpenAI node, which uses a system prompt to act as an SEO and content generator, and the resulting content is returned with a 200 status. If the key is invalid, the workflow terminates by responding with a 401 Unauthorized error.

## Output Details
The workflow returns an HTTP response directly to the calling client, containing either the AI-generated content (on success) or a 401 Unauthorized error message (on failed API key validation).
