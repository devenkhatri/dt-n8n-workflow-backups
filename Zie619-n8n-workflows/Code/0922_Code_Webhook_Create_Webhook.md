# Workflow Analysis for Secure Webhook with Authentication and Validation

## Description
This workflow provides a secure public webhook endpoint that validates incoming requests by checking for a valid Bearer token in the Authorization header and ensuring all required fields are present in the request body. It returns appropriate HTTP responses (200 OK, 401 Unauthorized, or 400 Bad Request) based on the validation results.

## Input Details
The workflow is triggered by a POST request to a webhook URL, receiving HTTP headers (including Authorization) and a JSON request body.

## Process Summary
The workflow begins by setting configuration values like the expected Bearer token and required request body fields. It first checks if the incoming Authorization header matches the configured token. If not, it returns a 401 Unauthorized response. If authentication passes, it validates that all required fields defined in the configuration are present in the request body using a custom JavaScript function. If any required field is missing, it returns a 400 Bad Request response. If both checks pass, it constructs a success response and returns a 200 OK status.

## Output Details
The workflow produces a JSON HTTP response with either a success message (200 OK) or an error message (401 Unauthorized or 400 Bad Request) sent back to the webhook caller.

## Tags
webhook, authentication, validation, security, API, error handling, n8n
