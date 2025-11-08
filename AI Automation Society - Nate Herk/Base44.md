# Workflow Analysis for AI Automation Roadmap Generator and HTML Report Sender

## Description
This workflow receives a business process description via a webhook, uses AI to generate a detailed automation roadmap, converts it into a professional HTML report, and then emails the report to a specified recipient.

## Input Details
The workflow is triggered by a POST webhook request, expecting a JSON payload containing a "prompt" with the business process description and an "email" address for sending the report.

## Process Summary
First, a webhook receives the business process prompt and recipient email. Then, an AI Consultant agent analyzes the prompt to create an AI automation roadmap, outlining inefficiencies, a step-by-step implementation plan, and estimated ROI, using the OpenAI/O3 model. Next, a Style Agent transforms this roadmap into a professional, email-compatible HTML report, leveraging the Anthropic/Claude-Sonnet-4.5 model. Finally, the generated HTML report is sent as an email to the address provided in the initial webhook request.

## Output Details
The workflow produces and sends a comprehensive, professionally formatted HTML email report containing an AI automation roadmap to the email address specified in the webhook input.
