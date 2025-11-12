# Workflow Analysis for Social Media Analysis and Personalized Outreach Workflow

## Description
This workflow automatically analyzes a lead's LinkedIn and Twitter activity to generate and send a personalized email with a relevant collaboration idea, based on shared interests or activities between the lead and your company.

## Input Details
The workflow is triggered by new or updated rows in a Google Sheet containing lead information including LinkedIn URL, Twitter handle, name, and email, where the 'done' column is empty.

## Process Summary
The workflow starts by checking Google Sheet entries for leads that haven’t been processed yet. It retrieves the lead’s Twitter ID and recent tweets, and fetches their LinkedIn posts via RapidAPI. It limits both Twitter and LinkedIn data to the latest 10 posts. Using this data, along with predefined company information, it prompts an OpenAI model to generate a personalized email subject and HTML cover letter proposing a relevant collaboration. Finally, it sends the email to the lead (and CCs the sender) and marks the lead as processed in the Google Sheet.

## Output Details
The workflow sends a personalized HTML email to the lead with a generated subject and cover letter, CCs the sender, and updates the Google Sheet to mark the lead as processed.

## Tags
lead generation, social media analysis, personalized email, AI automation, LinkedIn, Twitter, OpenAI, Google Sheets, RapidAPI, outreach automation
