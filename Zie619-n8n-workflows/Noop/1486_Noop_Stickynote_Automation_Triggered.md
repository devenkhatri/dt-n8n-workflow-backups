# Workflow Analysis for Extract Personal Data Using Self‑Hosted Mistral NeMo LLM

## Description
This workflow receives a user message, sends it to a locally hosted Mistral‑NeMo model via Ollama to extract personal information according to a predefined JSON schema, automatically repairs any malformed output, validates the structure, and returns the extracted data.

## Input Details
Triggered manually (or via webhook) with a user request/message containing the text to be analysed.

## Process Summary
1. The Basic LLM Chain node sends a prompt to the Mistral‑NeMo model asking it to extract fields defined in the JSON schema. 2. The model’s response is fed to the Auto‑fixing Output Parser, which re‑asks the model with correction instructions if the output violates constraints. 3. The corrected response is validated by the Structured Output Parser against the manual JSON schema. 4. The Set node extracts the parsed JSON from the parser’s output. 5. If any step fails, the workflow routes to the Error Handler.

## Output Details
The workflow outputs the extracted personal data as a JSON object for downstream use or API response.

## Tags
automation,n8n,LLM,data extraction,Mistral,Ollama,structured parsing
