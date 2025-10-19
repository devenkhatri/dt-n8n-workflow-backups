# Workflow Analysis for Webhook Triggered AI Text Translator

## Description
This workflow acts as an API endpoint, receiving text and a target language via a webhook, translating the text using an AI service, and immediately returning the translated content as an API response.

## Input Details
The workflow is triggered by a webhook that receives a JSON payload containing the text to be translated and the desired target language.

## Process Summary
The workflow starts by receiving the text and language data via a Webhook trigger. The input data is passed to an OpenAI node, which utilizes a language model to perform the translation task. A subsequent Set node processes and formats the AI output, isolating the final translated string. The process concludes by sending the translated text back to the caller as an HTTP response.

## Output Details
The workflow returns the translated text content in a JSON format directly back to the system that initiated the webhook call.
