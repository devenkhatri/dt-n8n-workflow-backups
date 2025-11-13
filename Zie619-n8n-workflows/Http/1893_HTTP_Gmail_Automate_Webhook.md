# Workflow Analysis for My workflow 3

## Description
This workflow automates the process of fetching SEO data, generating a report, and emailing it, ensuring efficient monitoring of website performance with robust error handling and security.

## Input Details
The workflow is triggered weekly every Monday at 7 AM by a scheduled cron job.

## Process Summary
The workflow starts with a weekly schedule on Monday mornings. It then makes an HTTP request to retrieve SEO data from Google Search Console. Next, a function node processes the retrieved SEO data to generate a formatted report detailing top search queries with clicks, impressions, CTR, and position. Finally, this generated SEO report is sent as an email.

## Output Details
The workflow sends a weekly SEO report via email to "rodrigue.gbadou@gmail.com".

## Tags
automation, n8n, production-ready, excellent, optimized
