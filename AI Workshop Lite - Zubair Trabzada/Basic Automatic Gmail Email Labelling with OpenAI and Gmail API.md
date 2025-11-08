# Workflow Analysis for AI-Powered Gmail Email Categorization

## Description
This workflow automatically sorts and labels incoming Gmail emails using an AI agent. It either assigns existing labels based on email content or creates new, structured labels when no suitable match is found, helping to keep your inbox organized.

## Input Details
The workflow is triggered every 5 minutes by new incoming emails in Gmail, receiving the email's metadata.

## Process Summary
The workflow first waits for a new email from Gmail. Then, an AI agent leverages an OpenAI chat model and several Gmail tools to analyze the email's content and existing labels. It decides whether to assign an existing label, create a new sub-label (under 'AI' or an existing main label), or remove the inbox label for promotional emails. Finally, it applies the chosen labels to the email in Gmail.

## Output Details
The workflow updates Gmail by categorizing emails with relevant labels and potentially creating new labels as needed.
