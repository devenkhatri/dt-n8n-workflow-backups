# Workflow Analysis for Create Fastmail Masked Email via Webhook

## Description
This workflow allows users to automatically generate a disposable masked email address through Fastmail's API by sending a webhook request with optional description and state parameters.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint with a JSON payload that may include 'state' and 'description' fields.

## Process Summary
The workflow starts by receiving a webhook request containing optional state and description for the masked email. It retrieves session information from the Fastmail API using authenticated HTTP headers. Using this session data, it constructs and sends a JMAP API request to create a new masked email with the provided details. Once the email is created, the workflow extracts the generated email address and description. Finally, it sends this information back as a response to the original webhook request.

## Output Details
The workflow responds directly to the incoming webhook with a JSON object containing the newly created masked email address and its description.

## Tags
fastmail, masked email, webhook, email privacy, disposable email, JMAP API, automation, n8n
