# Workflow Analysis for Extract personal data with a self-hosted LLM Mistral NeMo

## Description
Automated workflow: Extract personal data with a self-hosted LLM Mistral NeMo. This workflow integrates 8 different services: stickyNote, chainLlm, outputParserStructured, set, outputParserAutofixing. It contains 13 nodes and follows best practices for error handling and security.

## Input Details
The workflow is triggered either manually or by receiving a chat message via a webhook, which provides the user request for analysis.

## Process Summary
The workflow analyzes the incoming user request using a Basic LLM Chain, instructing a self-hosted Ollama Chat Model (Mistral NeMo) to extract information based on a predefined JSON schema. A Structured Output Parser then validates the LLM's response against this schema, which defines fields like name, surname, communication type, contacts, timestamp, and subject. If the LLM's output does not conform to the schema, an Auto-fixing Output Parser re-engages the LLM with a corrective prompt. The workflow extracts structured personal data, ensuring it adheres to the specified JSON format, with error handling to correct invalid responses.

## Output Details
The workflow produces extracted personal data in a structured JSON format, making it available for further use within the workflow or as a final output.

## Tags
automation,n8n,production-ready,excellent,optimized
