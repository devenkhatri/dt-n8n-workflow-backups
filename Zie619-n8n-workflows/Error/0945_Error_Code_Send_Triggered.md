# Workflow Analysis for Error Alert and Summarizer

## Description
This workflow automatically detects errors in n8n workflow executions, analyzes them using AI, and sends a detailed diagnostic email to designated recipients with actionable insights.

## Input Details
The workflow is triggered automatically whenever an error occurs in any n8n workflow execution.

## Process Summary
When an error occurs, the workflow captures the full execution data and extracts relevant error details while excluding specific nodes (e.g., SERP-related). It then sends this data to an AI model (OpenAI GPT-4o) with instructions to diagnose the issue, identify the root cause, and suggest a resolution. The AI's structured response is parsed and enriched with metadata like workflow and execution links. Finally, a formatted HTML email is generated and sent via Gmail to configured recipients.

## Output Details
The workflow sends a detailed HTML email to specified TO, CC, and BCC addresses containing diagnosis, cause, resolution, and links to the affected workflow and execution.

## Tags
error handling, AI analysis, email alert, n8n automation, OpenAI, workflow monitoring, production-ready
