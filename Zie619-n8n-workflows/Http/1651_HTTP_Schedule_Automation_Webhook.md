# Workflow Analysis for Gratitude Jar Reminder

## Description
This automated workflow helps users practice gratitude by sending daily reminders.

## Input Details
The workflow is triggered daily at 9:00 PM by a schedule.

## Process Summary
The workflow starts by triggering daily at 9:00 PM. It then uses an AI chat model (Azure OpenAI) to generate varied gratitude reminder messages to avoid repetition. The generated message is subsequently reformatted to ensure proper display by removing markdown and escaping newlines. Finally, this customized reminder is prepared for delivery.

## Output Details
The workflow sends a gratitude reminder message as a push notification to a user's LINE account.

## Tags
automation, n8n, production-ready, excellent, optimized
