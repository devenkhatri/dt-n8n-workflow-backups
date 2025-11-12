# Workflow Analysis for Production Workflow

## Description
This workflow securely processes an incoming webhook request by validating and transforming a CRC token using HMAC-SHA256 encryption, then returns a formatted response token. It is designed for production use with robust error handling.

## Input Details
The workflow is triggered by an HTTP webhook request containing a query parameter 'crc_token'.

## Process Summary
The workflow starts by receiving a webhook request. It extracts the 'crc_token' from the query parameters and computes an HMAC-SHA256 hash using a secret key from environment variables. The resulting hash is then formatted into a string 'sha256=<hash>' and stored as 'response_token'. Only this response token is kept in the output. If any step fails, the workflow triggers an error handler that stops execution and returns an error message.

## Output Details
The workflow outputs a JSON object containing the 'response_token' in the format 'sha256=<base64-encoded HMAC-SHA256 hash>', which is returned as the webhook response.

## Tags
webhook, security, HMAC, SHA256, token validation, production, error handling, n8n
