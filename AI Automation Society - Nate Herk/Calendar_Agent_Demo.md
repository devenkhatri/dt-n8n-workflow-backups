# Workflow Analysis for Automated Calendar Management and Email Outreach

## Description
This workflow automates calendar management and email outreach by leveraging AI to understand user requests, interact with Google Calendar, and send personalized emails.

## Input Details
The workflow is triggered by an HTTP request containing a prompt for the AI agent.

## Process Summary
The workflow starts by receiving an HTTP request with a prompt. It then uses a large language model to create a structured calendar query from the prompt, which is then used to interact with Google Calendar to add, update, or find events. After processing the calendar request, another large language model generates a personalized email based on the calendar action. Finally, the workflow sends this email.

## Output Details
The workflow sends a personalized email based on calendar actions and returns an HTTP response indicating the outcome.
