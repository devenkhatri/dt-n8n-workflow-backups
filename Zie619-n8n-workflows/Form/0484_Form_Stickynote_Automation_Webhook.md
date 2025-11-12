# Workflow Analysis for Dynamic credentials using expressions

## Description
This workflow demonstrates how to dynamically set API credentials using user-provided input via a web form, specifically for accessing NASA's API. It allows users to enter their NASA API key through a form, which is then securely passed to the NASA node using n8n expressions, enabling personalized API access without hardcoding credentials.

## Input Details
The workflow is triggered by a web form submission that collects the user's NASA API key.

## Process Summary
The workflow starts with a form trigger that asks the user to input their NASA API key. This key is captured in the workflow data. The NASA node then uses an expression in its credentials configuration to dynamically reference the submitted API key. The node fetches data from NASA’s API (such as the picture of the day) using this key. Finally, the workflow redirects the user to the NASA image URL via a webhook response.

## Output Details
The workflow redirects the user’s browser to NASA’s picture of the day (or related API result) using the provided API key.

## Tags
nasa, dynamic credentials, expressions, form trigger, api key, webhook, redirect, n8n
