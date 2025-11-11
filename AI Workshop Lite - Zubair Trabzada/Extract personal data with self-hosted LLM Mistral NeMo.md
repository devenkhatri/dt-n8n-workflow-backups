# Workflow Analysis for Extract personal data with a self-hosted LLM Mistral NeMo

## Description
This workflow uses a self-hosted Mistral NeMo large language model (via Ollama) to extract structured personal information—such as name, contact method, and communication details—from incoming chat messages.

## Input Details
The workflow is triggered when a chat message is received via a webhook.

## Process Summary
When a chat message arrives, it is passed to a Basic LLM Chain that uses the Mistral NeMo model hosted on Ollama to analyze the message and extract data according to a predefined JSON schema. The output is validated by a Structured Output Parser, and if it fails validation, an Auto-fixing Output Parser retries with a corrective prompt. Once valid, the extracted JSON is outputted for further use.

## Output Details
The workflow outputs a clean, structured JSON object containing the extracted personal data, which can be used by downstream systems or stored for record-keeping.

## Tags
LLM, Mistral NeMo, Ollama, personal data extraction, structured output, chat processing, self-hosted AI
