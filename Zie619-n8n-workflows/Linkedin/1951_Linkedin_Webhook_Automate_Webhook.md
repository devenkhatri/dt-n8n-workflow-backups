# Workflow Analysis for Training Feedback Automation

## Description
This n8n workflow automates the management of training feedback by integrating Airtable, Usertask, and various notification actions. It processes new or updated feedback entries from Airtable and webhook events from Usertask to ensure timely responses and improvements to training programs.

## Input Details
This workflow triggers hourly by new or updated training feedback entries in Airtable, or by a webhook receiving task results from Usertask.

## Process Summary
The workflow initiates by fetching new or updated training feedback from Airtable or by receiving a Usertask result via a webhook. It then uses a switch node to evaluate the feedback rating. Based on the rating, it creates specific tasks in Usertask for follow-up, such as urgent attention for poor feedback or general follow-up for fair and good feedback. For positive feedback, it generates a recognition post on LinkedIn. Finally, the workflow sends email notifications to relevant stakeholders, including trainers, HR, and marketing, providing updates on tasks or positive feedback.

## Output Details
The workflow creates tasks in Usertask, posts recognition on LinkedIn for positive feedback, and sends email notifications to relevant internal teams.

## Tags
automation, n8n, production-ready, excellent, optimized, Airtable, Usertask, LinkedIn, Email, Feedback, Training
