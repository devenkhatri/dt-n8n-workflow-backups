# Workflow Analysis for Suspicious Login Detection

## Description
This workflow detects and analyzes suspicious login attempts to identify potential security threats.

## Input Details
The workflow is triggered by a webhook receiving login event data.

## Process Summary
The workflow extracts relevant data from the login event, checks for IP trust with GreyNoise, and analyzes geolocation and user agent information. It then checks for anomalies in login location and device/browser usage, and assigns a priority level to the alert. The workflow also notifies the security team via Slack and emails the user if the login attempt is deemed suspicious.

## Output Details
The workflow produces an alert with priority level and sends notifications to the security team and the user.

## Tags
suspicious login detection, security, authentication, n8n, automation, workflow, greyNoise, IP-API, UserParser, slack, email, priority level, anomaly detection, geolocation, user agent, device/browser analysis
