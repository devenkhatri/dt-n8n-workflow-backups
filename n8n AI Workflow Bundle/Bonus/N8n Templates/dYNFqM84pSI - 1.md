# Workflow Analysis for AI-Powered n8n Workflow Analyzer and Documenter

## Description
This workflow automates the documentation process for any n8n workflow by using the OpenAI GPT-4 model to analyze the workflow's JSON structure and extract key details like the title, description, and process summary. Once the analysis is complete, it sends notifications via both Telegram and Email with the comprehensive documentation.

## Input Details
The workflow is triggered by an incoming HTTP request to a webhook, which is expected to contain the n8n workflow JSON structure to be analyzed.

## Process Summary
The workflow starts when a webhook is received containing the target workflow's JSON data. This JSON is passed to the OpenAI node, which uses GPT-4 and a specific prompt to analyze the workflow and generate structured documentation details. Finally, the generated documentation, including the title, summary, and tags, is broadcasted to both a designated Telegram chat and a specified email address via Mailgun.

## Output Details
The workflow generates structured documentation of the input workflow and sends comprehensive notifications containing this documentation via Telegram and Email (using Mailgun).
