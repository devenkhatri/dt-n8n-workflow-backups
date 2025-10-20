# Workflow Analysis for RabbitMQ SMS Alert System

## Description
This workflow monitors a RabbitMQ queue for new messages and sends an SMS alert using Twilio for each message received.

## Input Details
This workflow is triggered when a new message is received in a specified RabbitMQ queue.

## Process Summary
The workflow starts by listening for new messages in a RabbitMQ queue. Upon receiving a message, it extracts the message content. Then, a Twilio node is used to send an SMS alert to a predefined phone number, using the extracted message content as the SMS body.

## Output Details
The workflow sends an SMS alert via Twilio for each message received from the RabbitMQ queue.
