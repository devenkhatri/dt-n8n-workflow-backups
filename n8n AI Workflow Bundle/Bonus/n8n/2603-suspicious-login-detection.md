# Workflow Analysis for Suspicious Login Detection

## Description
This workflow detects suspicious login attempts by analyzing login data, enriching it with IP address information, and using OpenAI to determine if the login is suspicious. If a login is deemed suspicious, it sends a notification.

## Input Details
The workflow is triggered by an HTTP request, receiving login event data as its input.

## Process Summary
The workflow starts by receiving login data. It then extracts the IP address from the login data and retrieves geographic information for that IP. Next, it combines the login and IP data into a single object. Finally, it uses OpenAI to assess if the login is suspicious based on the combined information.

## Output Details
The workflow sends notifications via Telegram or Discord if a suspicious login is detected.
