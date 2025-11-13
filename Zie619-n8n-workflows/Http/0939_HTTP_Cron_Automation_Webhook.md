# Workflow Analysis for NameCheap Dynamic DNS (DDNS)

## Description
This workflow automatically updates DNS records for specified subdomains on NameCheap whenever your public IP address changes, ensuring your domain always points to your current IP.

## Input Details
The workflow is triggered on a schedule (every 15 minutes) and fetches the current public IP address from an external service.

## Process Summary
The workflow starts by fetching the current public IP address. It then checks if this IP is different from the previously recorded one using global static data. If the IP has changed, it proceeds to define a list of subdomains to update. For each subdomain, it prepares the domain and authentication details, then sends an update request to NameCheap's DDNS API.

## Output Details
The workflow sends HTTP requests to NameCheap's DDNS service to update DNS records for each configured subdomain with the new IP address.

## Tags
NameCheap, DDNS, Dynamic DNS, IP monitoring, automation, scheduled workflow, DNS update
