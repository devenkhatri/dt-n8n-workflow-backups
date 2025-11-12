# Workflow Analysis for puq-docker-immich-deploy

## Description
This workflow provides a managed API for deploying, controlling, and monitoring Immich (a self-hosted photo backup service) Docker containers on a remote server. It supports operations like creating, starting, stopping, suspending, and terminating Immich instances, as well as fetching container stats, logs, user data, and managing access control lists (ACLs).

## Input Details
The workflow is triggered by a POST webhook request containing a JSON payload with command instructions (e.g., create, start, stop), server domain, and configuration parameters like disk size, CPU, RAM, and credentials.

## Process Summary
The workflow begins by validating the incoming server domain. Based on the command in the request, it routes execution through switch nodes to perform specific actions. These actions include generating Docker Compose files and NGINX configurations, executing shell scripts via SSH to manage containers, disks, and services, and retrieving system or application data. The scripts handle tasks like mounting disks, starting/stopping containers, deploying new instances, changing packages, managing ACLs, and fetching logs or user lists. A final code node parses the SSH command output and formats a standardized JSON response.

## Output Details
The workflow returns a JSON response to the webhook caller indicating success or error, along with relevant data such as container stats, logs, user lists, or status messages.

## Tags
docker, immich, automation, ssh, webhook, container management, server automation, n8n, infrastructure as code, api backend
