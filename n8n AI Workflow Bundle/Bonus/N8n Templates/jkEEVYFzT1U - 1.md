# Workflow Analysis for Real-time AI Sentiment and Text Analysis Webhook

## Description
This workflow is designed to receive a piece of text via a webhook, use an AI model (OpenAI) to perform detailed sentiment analysis, generate a concise summary, and extract key points, and then immediately return the structured analysis results to the sender.

## Input Details
The workflow is triggered by an incoming HTTP request (a Webhook) that is expected to contain a 'text' field in its body.

## Process Summary
The workflow is initiated by an incoming HTTP Webhook request containing the text to be analyzed. It first extracts the input text from the request body. This text is then passed to an OpenAI Chat node, which uses a specific system prompt to perform sentiment analysis, summarization, and key point extraction, generating a clean JSON output. A subsequent Set node prepares this structured data. Finally, the analysis result is immediately sent back to the originator as the response to the initial Webhook call.

## Output Details
The workflow returns a structured JSON response to the triggering webhook containing the text analysis, including the sentiment (Positive, Negative, or Neutral), a summary, and a list of key points.
