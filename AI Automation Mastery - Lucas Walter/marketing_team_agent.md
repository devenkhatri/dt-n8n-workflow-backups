# Workflow Analysis for Marketing Team AI Assistant with n8n and OpenAI

## Description
This workflow automates the process of generating marketing content using AI, triggered by a webhook with a specific prompt, and then shares the generated content via email and Notion.

## Input Details
The workflow is triggered by an HTTP webhook that receives a POST request containing a "prompt" in its body.

## Process Summary
First, the workflow receives a prompt via a webhook. Then, it uses this prompt to query an OpenAI GPT-4 model, instructing it to act as a marketing assistant and generate marketing content. Next, it extracts the generated content, summarizes it, and constructs an email with the content. Finally, the workflow sends this email through Gmail and creates a new page in Notion containing the generated marketing content.

## Output Details
The workflow sends an email with the generated marketing content via Gmail and creates a new page in Notion with the content.
