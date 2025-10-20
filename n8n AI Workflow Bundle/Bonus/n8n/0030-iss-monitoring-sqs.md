# Workflow Analysis for ISS Location Monitoring and SQS Notification

## Description
This workflow tracks the International Space Station (ISS) location, checks if it is over a specified country, and sends a message to an SQS queue if it is.

## Input Details
This workflow is triggered every five minutes by a cron job.

## Process Summary
The workflow starts by retrieving the current location of the ISS from an external API. Then, it uses a geographic lookup service to determine the country and county the ISS is currently over. If the ISS is over the specified country (Turkey in this case), the workflow constructs a message containing the ISS location data. Finally, this message is sent to an AWS SQS queue.

## Output Details
The workflow sends a message containing ISS location data to an AWS SQS queue when the ISS is over Turkey.
