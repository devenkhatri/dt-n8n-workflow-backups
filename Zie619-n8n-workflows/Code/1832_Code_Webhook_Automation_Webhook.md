# Workflow Analysis for PUQ Docker NextCloud deploy

## Description
This workflow provides a fully automated API backend for deploying, managing, and monitoring Docker-based NextCloud instances integrated with WHMCS/WISECP. It handles provisioning, suspending, resuming, terminating, and modifying server resources, along with DNS management and container-level operations such as starting/stopping, disk mounting, log retrieval, and user/password management.

## Input Details
Triggered by a POST request to a secured webhook endpoint with JSON payload containing domain, server details, resource specs, and a command (e.g., create, suspend, change_package).

## Process Summary
The workflow first validates the server domain and sets key path parameters. It then routes execution based on the requested command: deploying or modifying NextCloud instances, managing container lifecycle (start/stop/mount), fetching stats/logs, handling DNS records via external API, or performing NextCloud-specific actions like fetching users or changing passwords. Shell scripts are dynamically generated and executed via SSH on the target server (d01-test.uuq.pl or d02-test.uuq.pl), and results are parsed and returned as structured JSON responses.

## Output Details
Returns a JSON response to the webhook caller indicating success or error, optionally including detailed data such as container stats, logs, user lists, or version info.

## Tags
NextCloud, Docker, automation, WHMCS, WISECP, server management, container orchestration, DNS integration, n8n, production-ready
