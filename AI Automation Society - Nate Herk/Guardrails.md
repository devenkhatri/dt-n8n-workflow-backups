# Workflow Analysis for Guardrails Workflow

## Description
This n8n workflow demonstrates the functionality of Guardrail nodes to add control and reliability to workflows involving AI or user inputs. It showcases various text checking and sanitization capabilities across different categories like keywords, jailbreak attempts, NSFW content, personal identifiable information (PII), secret keys, topical alignment, and URL validation.

## Input Details
The workflow receives predefined sets of text strings as input from multiple "Edit Fields" (Set) nodes, which are then processed individually for demonstration purposes.

## Process Summary
The workflow processes different sets of input texts, each split into individual items. These items are then passed through various Guardrail nodes to check for specific violations such as containing keywords, being a jailbreak attempt, including NSFW content, detecting PII, revealing secret keys, verifying topical alignment, and validating URLs. Additionally, it demonstrates sanitization operations for PII, secret keys, and URLs by masking or removing sensitive information from the input text.

## Output Details
The workflow outputs the results from each Guardrails node, indicating whether the input text triggered a specific guardrail violation (e.g., "Flagged") or, in the case of sanitization, the modified (sanitized) text.

## Tags
Guardrails, Text Analysis, Content Moderation, AI, LLM, Security, PII, Jailbreak, Keywords, URLs, Sanitization
