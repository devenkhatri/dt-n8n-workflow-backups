# Workflow Analysis for Send Log Entries to BetterStack

## Description
This workflow sends structured log messages to BetterStack Logs for centralized monitoring and debugging. It can be called from other workflows or used as a standalone utility for logging events with a specified severity level and message content.

## Input Details
The workflow is triggered either manually for testing or via another workflow that passes a 'level' (e.g., error, info) and a 'message' as input parameters.

## Process Summary
The workflow receives a log level and message as inputs. It then formats these into a JSON payload. Using an HTTP Request node, it sends this payload to a BetterStack Logs endpoint with authentication via a Bearer token in the header. The workflow includes robust error handling through multiple error-handler nodes. Additionally, it provides a test path using a manual trigger that simulates sending a sample log message.

## Output Details
The workflow sends a POST request to BetterStack Logs containing the log message and severity level, enabling centralized logging and monitoring.

## Tags
logging, BetterStack, error tracking, workflow utility, n8n, HTTP request, monitoring, centralized logging
