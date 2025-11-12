# Workflow Analysis for Weekly Shodan Query - Report Accidents (no function node)

## Description
This workflow automatically scans a list of monitored IP addresses and their expected ports using Shodan every Monday to detect any unexpected open ports. If any unexpected ports are found, it formats the findings into a Markdown table and creates a security alert in TheHive for immediate investigation.

## Input Details
The workflow is triggered every Monday at 5 AM UTC and receives a list of IP addresses with their expected ports from an external security system via an HTTP request.

## Process Summary
The workflow starts by fetching a list of monitored IPs and their expected ports from a security system. It then processes each IP individually, querying Shodan to retrieve all open ports and services running on that IP. The services are split into individual items, and each port is checked against the list of expected ports. If a port is not in the expected list, it is flagged as unexpected, formatted into a structured data object, converted to an HTML table, and then to Markdown. Finally, an alert is created in TheHive with the formatted findings.

## Output Details
The workflow creates security alerts in TheHive for any IPs with unexpected open ports, including a Markdown-formatted report of the findings.

## Tags
security, shodan, thehive, port scanning, weekly report, IP monitoring, n8n, automation, incident response, markdown
