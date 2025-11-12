# Workflow Analysis for puq-docker-minio-deploy

## Description
This workflow provides a complete API backend for managing Docker-deployed MinIO instances, supporting actions like creating, starting, stopping, suspending, and resizing MinIO containers along with disk and network management. It is designed to integrate with hosting control panels like WHMCS or WISECP.

## Input Details
The workflow is triggered by a POST webhook request containing a command (e.g., create, start, stop) and parameters such as domain, disk size, CPU, and RAM allocation for a MinIO instance.

## Process Summary
The workflow first validates the incoming server domain and command. Based on the command, it routes execution to specific actions such as deploying a new MinIO container, starting or stopping containers, mounting or unmounting disk images, managing access control lists (ACLs), retrieving logs or stats, or changing service packages. It generates necessary configuration files (docker-compose, NGINX), executes shell commands via SSH on a remote Docker host, and formats the results. Finally, it returns a structured JSON response indicating success or error.

## Output Details
The workflow responds directly to the triggering webhook with a JSON payload indicating the operation status (success or error), a message, and optionally returned data such as container stats, logs, or user lists.

## Tags
MinIO, Docker, automation, hosting, WHMCS, WISECP, API, container management, n8n, infrastructure, S3
