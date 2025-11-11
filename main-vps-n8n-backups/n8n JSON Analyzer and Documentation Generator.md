# Workflow Analysis for n8n JSON Analyzer and Documentation Generator

## Description
This workflow analyzes n8n workflow JSON files and automatically generates structured documentation including title, description, input/output details, process summary, and tags for better organization and understanding.

## Input Details
The workflow is triggered by a JSON file containing an n8n workflow definition, typically uploaded or provided via a webhook or file trigger.

## Process Summary
The workflow parses the input n8n JSON to extract key metadata and node configurations. It identifies the trigger type, input sources, processing steps, and output destinations. Using this information, it generates a human-readable documentation summary with a title, description, input/output details, and a step-by-step process overview. It also auto-generates relevant tags based on the workflow's functionality and nodes used. Finally, the structured documentation is formatted according to a predefined schema.

## Output Details
The workflow produces a formatted JSON object containing the generated documentation, which can be saved to a file, sent via API, or displayed in a UI for workflow cataloging or sharing.

## Tags
n8n, documentation, JSON analyzer, workflow automation, metadata extraction, documentation generator
