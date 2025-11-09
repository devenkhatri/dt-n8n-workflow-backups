# Workflow Analysis for AI Automation Consultant with HTML Report & Email Delivery

## Description
This workflow accepts a business process description via a webhook, analyzes it using an AI consultant to generate an automation roadmap, formats the response as a professional HTML report, and emails it to the provided address.

## Input Details
The workflow is triggered by a POST request to a webhook URL containing a JSON payload with a 'prompt' describing a business process and an 'email' address to send the report to.

## Process Summary
The workflow starts when a POST request is sent to the webhook endpoint. The 'AI Consultant' agent processes the prompt using the OpenAI o3 model to generate an automation roadmap. This output is then passed to the 'Style Agent', which uses Claude Sonnet 4.5 to format the content into a professional, email-ready HTML report with inline CSS. Finally, the formatted HTML is sent as an email to the address provided in the original webhook request using a Gmail account.

## Output Details
The workflow produces a professionally formatted HTML report containing an AI-generated automation roadmap and sends it as an email to the address specified in the input webhook request.

## Tags
AI Consultant, Automation Roadmap, HTML Report, Email Delivery, Webhook Trigger, OpenRouter, Gmail
