# Workflow Analysis for Receive messages from a queue via RabbitMQ and send an SMS

## Description
This workflow automatically processes messages received from a RabbitMQ queue and sends an SMS alert under specific conditions.

## Input Details
The workflow is triggered by messages received from a "temp" queue in RabbitMQ, which are then parsed as JSON.

## Process Summary
The workflow starts by receiving a message from the 'temp' queue in RabbitMQ. It then checks if the 'temp' value within the message is greater than 50. If true, an SMS alert is sent via Vonage with the 'temp' value. If false, the workflow proceeds without further action. An error handler is in place for general execution issues.

## Output Details
The workflow conditionally sends an SMS alert via Vonage if the 'temp' value in the RabbitMQ message is above 50.

## Tags
automation, n8n, production-ready, excellent, optimized
