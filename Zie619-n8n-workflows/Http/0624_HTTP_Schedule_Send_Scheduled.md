# Workflow Analysis for Httprequest Workflow

## Description
This workflow automatically checks for security alerts from an Elastic monitoring system at scheduled intervals and sends email notifications for each triggered alert with details like name, severity, timestamp, and message.

## Input Details
The workflow is triggered on a schedule and fetches alert data from an external API endpoint defined by the environment variable API_BASE_URL.

## Process Summary
The workflow starts with a scheduled trigger that initiates an HTTP request to retrieve Elastic alert data. It then checks if the response contains any alerts. If no alerts are found, the workflow ends. If alerts exist, it splits the alert list into individual items and loops through each one. For each alert, it sends a formatted HTML email notification via a POST request to a webhook URL using OAuth2 authentication.

## Output Details
The workflow sends individual email notifications for each active alert to a predefined recipient using a Microsoft Graph-compatible email API.

## Tags
automation, n8n, production-ready, alerting, email notification, elastic, security monitoring, scheduled workflow
