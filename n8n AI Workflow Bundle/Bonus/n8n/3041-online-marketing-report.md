# Workflow Analysis for Automated Online Marketing Report Generation

## Description
This workflow automates the generation and distribution of a weekly online marketing report, compiling data from various sources into a PDF and sending it via email.

## Input Details
The workflow is triggered once a week by a scheduled cron job.

## Process Summary
The workflow starts by setting the previous week's date range. It then queries Google Analytics and Google Search Console for performance data. This raw data is then processed and formatted into a structured report using HTML, which is then converted into a PDF document. Finally, the generated PDF report is attached to an email and sent to a specified recipient list.

## Output Details
The workflow produces a PDF online marketing report and sends it as an email attachment to a predefined list of recipients.
