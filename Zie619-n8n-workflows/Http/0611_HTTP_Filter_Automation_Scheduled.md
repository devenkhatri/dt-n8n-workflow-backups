# Workflow Analysis for DigitalOcean Droplet Snapshot Manager

## Description
This workflow automatically manages snapshots for DigitalOcean droplets by ensuring no more than 4 snapshots exist per droplet. It runs every 48 hours, deletes the oldest snapshot if the limit is exceeded, and creates a new snapshot to keep backups up to date.

## Input Details
The workflow is triggered automatically every 48 hours by a cron scheduler and does not require external input data.

## Process Summary
The workflow starts by listing all droplets in a DigitalOcean account. For each droplet, it retrieves the list of existing snapshots. It then checks if the number of snapshots is 4 or more. If so, it deletes the oldest snapshot. Finally, it creates a new snapshot for the droplet to ensure recent backups are maintained.

## Output Details
The workflow produces updated snapshot states for each droplet on DigitalOcean by deleting old snapshots and creating new ones, with all actions performed directly via API calls to DigitalOcean.

## Tags
DigitalOcean, snapshot management, automation, cron, backup, infrastructure, n8n, production-ready
