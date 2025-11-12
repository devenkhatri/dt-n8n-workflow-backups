# Workflow Analysis for puq-docker-n8n-deploy

## Description
This workflow provides a secure and automated API backend for managing Docker-based n8n instances integrated with WHMCS or WISECP billing platforms. It supports full lifecycle operations like creating, starting, stopping, suspending, and terminating client containers, as well as inspecting stats, managing disk mounts, updating ACLs, and changing service packages.

## Input Details
The workflow is triggered by a POST webhook request containing a JSON payload with a command (e.g., create, start, stop) and parameters like domain, disk size, CPU, RAM, and optional ACLs or user credentials.

## Process Summary
The workflow first validates the incoming server domain. It then routes the request based on the command to one of several specialized Switch nodes (Service Actions, Container Actions, Container Stats, or n8n-specific actions). Each path generates a custom shell script using Set nodes, which is executed via SSH on the target Docker host. The script performs tasks like deploying containers, managing disk mounts, updating Nginx configurations, or querying container stats. A Code node parses the SSH command output and formats the response before returning it to the caller.

## Output Details
The workflow returns a structured JSON response (success or error) to the original webhook caller, summarizing the result of the executed Docker or system operation.

## Tags
docker, n8n, automation, WHMCS, WISECP, container management, API backend, SSH, webhook, infrastructure automation
