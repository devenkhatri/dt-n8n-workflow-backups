# Workflow Analysis for Qualys Vulnerability Management via Slack Bot

## Description
This workflow automates vulnerability management by allowing users to query Qualys for host and vulnerability information directly from Slack using a slash command. It processes user input, retrieves relevant data from Qualys, and presents it in an easily digestible format within Slack, streamlining security operations.

## Input Details
The workflow is triggered by an HTTP POST request, typically from a Slack slash command, containing user input for host or vulnerability queries.

## Process Summary
The workflow starts by receiving a Slack command with a query. It then parses the user input to determine if it is a host IP or a vulnerability QID. Based on the input, it makes an API call to Qualys to retrieve either host details or vulnerability information. If no specific IP or QID is provided, it defaults to listing the top 10 vulnerabilities. Finally, it formats the retrieved data into a user-friendly message and sends it back to the Slack channel.

## Output Details
The workflow sends formatted messages containing Qualys host or vulnerability information back to the Slack channel from which the command originated.
