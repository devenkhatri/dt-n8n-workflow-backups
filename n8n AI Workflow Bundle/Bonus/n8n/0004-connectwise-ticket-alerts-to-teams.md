# Workflow Analysis for ConnectWise Ticket Alerts to Microsoft Teams

## Description
This workflow automates the process of sending ConnectWise ticket status updates as notifications to a specified Microsoft Teams channel.

## Input Details
The workflow is triggered by an HTTP POST request, typically from a ConnectWise webhook, containing ticket update information.

## Process Summary
The workflow starts by receiving an HTTP POST request containing ConnectWise ticket data. It then extracts relevant information such as ticket ID, summary, and status from the received data using a Set node. Next, it constructs a formatted message for Microsoft Teams using another Set node. Finally, it sends this formatted message as a notification to a designated Microsoft Teams channel.

## Output Details
The workflow sends a formatted notification message to a Microsoft Teams channel.
