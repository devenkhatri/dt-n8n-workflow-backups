# Workflow Analysis for n8n Assistant Tool

## Description
This workflow serves as an assistant tool for n8n, helping users understand and debug workflows by accepting a workflow JSON, analyzing it, and providing insights using AI.

## Input Details
The workflow is manually triggered and receives an n8n workflow JSON as input.

## Process Summary
The workflow starts by extracting the workflow JSON and determining if it needs to be fetched from a URL or is directly provided. It then converts the JSON to a string, encodes it into a buffer, and makes a request to OpenAI to analyze the workflow JSON. The OpenAI response is processed to extract key insights, which are then returned as the output.

## Output Details
The workflow outputs a JSON object containing the AI-generated analysis of the provided n8n workflow, including a title, description, input details, process summary, output details, and tags.
