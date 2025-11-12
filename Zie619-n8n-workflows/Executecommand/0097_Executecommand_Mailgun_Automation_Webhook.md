# Workflow Analysis for Steam + CF Report

## Description
This workflow automatically checks if a reported domain is associated with Cloudflare and, if so, sends alert emails to both Cloudflare and Steam (Valve Software) to report a potential phishing site impersonating Steam.

## Input Details
The workflow is triggered by an authenticated webhook that receives a domain name via a query parameter 'q'.

## Process Summary
First, it validates that the input domain contains only safe characters using a regex check. Then it ensures the system has the 'dig' DNS utility by installing bind-tools if needed. It checks if the domain has valid nameservers, and if so, performs a DNS lookup to see if Cloudflare is among them. If Cloudflare is detected, it sends an email to Cloudflare's security team; regardless of Cloudflare usage, it also sends a report to Steam's security team.

## Output Details
The workflow sends email notifications to security@cloudflare.com and security@valvesoftware.com with details about the suspected Steam phishing domain.

## Tags
steam, cloudflare, phishing detection, dns lookup, email alert, security report, automation
