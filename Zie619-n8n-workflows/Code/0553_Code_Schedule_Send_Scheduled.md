# Workflow Analysis for Ftp Workflow

## Description
This workflow automatically backs up Zigbee2MQTT configuration by requesting a backup via MQTT, processing the received backup data, and uploading it as a timestamped ZIP file to an SFTP server.

## Input Details
The workflow is triggered automatically every Monday at 2:45 AM via a cron schedule and receives a backup response from Zigbee2MQTT over MQTT.

## Process Summary
The workflow starts with a scheduled trigger that sends a backup request to Zigbee2MQTT via MQTT. It then listens for the backup response on a specific MQTT topic. Once received, it parses the JSON message to extract the base64-encoded ZIP data. This data is converted into a binary file, and finally, the file is uploaded to an SFTP server with a timestamped filename.

## Output Details
The workflow produces a ZIP backup file of Zigbee2MQTT configuration and uploads it to a designated SFTP directory with a unique timestamped name.

## Tags
zigbee2mqtt, backup, sftp, mqtt, automation, cron, file upload, json parsing, base64, production-ready
