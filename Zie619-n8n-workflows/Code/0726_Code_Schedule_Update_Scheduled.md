# Workflow Analysis for VPS Upgrade Notification

## Description
This workflow automatically checks your server daily for upgradable packages and sends an email notification if updates are available.

## Input Details
The workflow is triggered on a daily schedule and connects to a server via SSH to fetch a list of upgradable packages.

## Process Summary
The workflow starts with a daily schedule trigger, then connects to a server via SSH to run the command 'apt list --upgradable'. The output is formatted into an HTML list using a code node. An IF condition checks whether the list contains any packages (i.e., it's not empty). If updates are found, an email is sent via SMTP with the list of upgradable packages.

## Output Details
If upgradable packages are found, the workflow sends an HTML-formatted email to a configured recipient notifying them of available updates.

## Tags
server monitoring, package updates, SSH, email notification, automation, Linux, apt, scheduled workflow
