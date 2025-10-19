# Workflow Analysis for AI-Powered Text Summarization API Endpoint

## Description
This workflow exposes an API endpoint that accepts raw text, utilizes the OpenAI GPT model to generate a concise summary of the text, and returns the summary directly as an API response.

## Input Details
The workflow is triggered by an external HTTP POST request to a custom Webhook path (`/summarize`), expecting a JSON body containing the text to be summarized.

## Process Summary
The workflow starts by accepting a text input via a Webhook trigger set to the `/summarize` path. A 'Set Text' node extracts the raw text from the incoming JSON body. The extracted text is then passed to the OpenAI node, which uses a pre-defined system message to perform text summarization using the GPT model. Finally, the generated summary from the OpenAI response is extracted and directly returned as the response body to the original webhook request.

## Output Details
The workflow returns the AI-generated text summary as a JSON response to the original HTTP client that triggered the webhook.
