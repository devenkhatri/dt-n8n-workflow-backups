# Workflow Analysis for Suspicious Login Detection

## Description
This workflow detects and analyzes suspicious login attempts by combining data from various sources like GreyNoise, IP-API, and UserParser, and then notifies users via email about unusual login activities.

## Input Details
The workflow is triggered by a webhook receiving data from login events, capturing vital information such as IP addresses and user details.

## Process Summary
The workflow extracts relevant data from the login event, checks the IP address against GreyNoise and IP-API for geolocation insights, parses user agent data, and merges all the information for comprehensive analysis. It then checks for anomalies in location and device/browser usage, assigns priority levels based on the analysis, and routes the workflow accordingly. The workflow can notify users via email about unusual login activities and can also send notifications to Slack for immediate attention.

## Output Details
The workflow produces email notifications to users about unusual login activities and sends notifications to Slack for immediate attention, ensuring prompt action against potential security threats.

## Tags
security, login detection, anomaly detection, email notification, Slack notification, GreyNoise, IP-API, UserParser
