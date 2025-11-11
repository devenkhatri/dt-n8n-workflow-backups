# Workflow Analysis for AI Email Reply and Feedback Collection

## Description
This workflow automatically replies to incoming emails using OpenAI's GPT model and collects user feedback on the AI responses. It saves both the original messages and AI replies to a Google Sheet for potential model fine-tuning.

## Input Details
The workflow is triggered either by receiving an email in Gmail or by a user clicking a feedback link in a previously sent AI-generated email reply.

## Process Summary
When an email is received, the workflow checks if it's from an approved sender, extracts the message content, and generates an AI reply using OpenAI. It then sends the reply back to the sender with embedded feedback links (Yes/No). Both the original message and AI response are saved to a Google Sheet, creating the spreadsheet if it doesn't exist. When a user clicks a feedback link, the workflow captures this response and updates the corresponding record in the Google Sheet.

## Output Details
The workflow sends an AI-generated email reply to the original sender and stores all email exchanges and feedback in a Google Sheet for analysis and potential model fine-tuning.

## Tags
AI,email automation,OpenAI,Gmail,Google Sheets,feedback collection,workflow automation,n8n
