# Workflow Analysis for Facebook Ad Thief with AI Summarization

## Description
This workflow automates the process of extracting Facebook ad data, enriching it with company information, and then summarizing the ad copy using AI, finally compiling a detailed report in a Google Sheet and sending it via email.

## Input Details
The workflow is triggered manually or on a schedule to initiate the ad extraction process.

## Process Summary
The workflow starts by retrieving Facebook ad data and then uses a custom API to get company information based on a domain. It then uses OpenAI to summarize the ad copy and generate a concise report based on the ad creative. Finally, it uses a custom Python script to prepare the ad and company data and saves it into a Google Sheet as a new row. Upon successful completion, an email notification is sent with the updated Google Sheet.

## Output Details
The workflow produces a new row in a specified Google Sheet containing detailed ad information and a summary, and sends an email notification with a link to the updated sheet.
