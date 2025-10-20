# Workflow Analysis for MCP Manager Workflow

## Description
This workflow manages MCPE (Minecraft Pocket Edition) servers by starting, stopping, and running commands on them through pterodactyl.

## Input Details
The workflow is triggered manually and receives commands to manage Minecraft servers.

## Process Summary
The workflow begins by manually receiving server management commands. It then authenticates with the Pterodactyl API and retrieves server details using a server ID. Based on the specified command (uninstall, suspend, power_stop, power_start, send_command), it executes the corresponding action on the Minecraft server using the Pterodactyl API. Finally, it logs the success or failure of the operation.

## Output Details
The workflow outputs the results of the server management operations to the console and handles errors by sending a notification via the Gotify service.
