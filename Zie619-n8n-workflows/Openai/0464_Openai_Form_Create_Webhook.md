# Workflow Analysis for Workflow Documenter

## Description
This workflow automates the creation of comprehensive documentation for n8n workflows by leveraging AI. It takes a workflow's title and JSON definition and generates a detailed description, use case, setup guide, and customization instructions, following specific guidelines for clarity and SEO.

## Input Details
The workflow is triggered by an n8n form submission, receiving the workflow title and its JSON definition as input.

## Process Summary
First, the workflow receives a workflow title and JSON via an n8n form. Next, it prepares a detailed prompt for an AI model, outlining the requirements for generating workflow documentation. This prompt, along with the submitted workflow title and JSON, is then fed into an OpenAI GPT-4 model. Finally, the AI-generated workflow documentation is formatted into an HTML response and returned via a webhook.

## Output Details
The workflow produces AI-generated, detailed documentation for an n8n workflow and returns it as an HTML response via a webhook.

## Tags
automation, n8n, production-ready, excellent, optimized, documentation, AI
