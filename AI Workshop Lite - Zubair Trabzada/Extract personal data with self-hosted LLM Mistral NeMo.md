# Workflow Analysis for Extract Personal Data with Self-Hosted LLM

## Description
This workflow uses a self-hosted Large Language Model (LLM), Mistral NeMo, to extract personal data from incoming chat messages. It ensures the extracted data adheres to a predefined JSON schema, with an auto-fixing mechanism to correct any non-compliant outputs.

## Input Details
The workflow is triggered when a chat message is received, and it processes the content of this message.

## Process Summary
Upon receiving a chat message, the workflow sends it to a Basic LLM Chain. This chain utilizes a self-hosted Ollama Chat Model (Mistral NeMo) to analyze the message. A Structured Output Parser defines a specific JSON schema for extracting personal information such as name, surname, communication type, contact details, timestamp, and subject. An Auto-fixing Output Parser is integrated to re-prompt the LLM if its initial response fails to conform to the defined JSON schema, ensuring data consistency. Finally, the extracted and validated structured JSON data is prepared as the workflow's output.

## Output Details
The workflow produces a structured JSON output containing extracted personal data (name, surname, communication type, contacts, timestamp, subject) from the chat message.
