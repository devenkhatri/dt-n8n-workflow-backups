# Workflow Analysis for Openai Workflow

## Description
This workflow automatically replies to incoming emails using OpenAI's GPT, saves both the original message and AI-generated reply to a Google Sheet, and collects user feedback on the AI's response quality for potential model fine-tuning.

## Input Details
The workflow is triggered either by receiving an email via Gmail or by a user clicking a feedback link in an AI-generated email reply.

## Process Summary
When an email is received, the workflow checks if it's from an approved sender, extracts the message content, and checks if it's within token limits. If valid, it sends the content to OpenAI to generate a reply. The reply is sent back to the sender with embedded feedback links (Yes/No). Both the original message and AI reply are saved to a Google Sheet, creating the sheet if it doesn't exist. When a user clicks a feedback link, the workflow records their response (positive or negative) in the same Google Sheet against the relevant message using a unique ID.

## Output Details
The workflow sends an AI-generated email reply with feedback links and stores message data and feedback in a Google Sheet for analysis and potential AI model fine-tuning.

## Tags
AI, email automation, OpenAI, GPT, Gmail, Google Sheets, feedback collection, auto-reply, workflow automation, n8n
