# Workflow Analysis for Social Media Analysis and Personalized Outreach Workflow

## Description
This workflow automatically analyzes a lead's LinkedIn and Twitter activity to generate and send a personalized email based on shared interests or potential collaboration opportunities, using AI to craft the message.

## Input Details
The workflow is triggered by new or updated rows in a Google Sheet containing lead information including LinkedIn URL, Twitter handle, name, and email, where the 'done' column is empty.

## Process Summary
The workflow starts by reading lead data from a Google Sheet. It then fetches the lead's Twitter ID and recent tweets, as well as their LinkedIn posts, using RapidAPI. The retrieved posts are limited to 10 each and formatted. An AI model (OpenAI) analyzes this social media data along with company information (name, activity, contact) to generate a personalized email subject and HTML cover letter. Finally, the email is sent to the lead with a CC to the sender, and the Google Sheet is updated to mark the row as processed.

## Output Details
The workflow sends a personalized HTML email to the lead (and CCs the sender) and updates the corresponding row in the Google Sheet with a 'done' marker.

## Tags
social media analysis, lead generation, personalized email, AI content generation, LinkedIn automation, Twitter automation, Google Sheets integration, outbound outreach, n8n workflow, marketing automation
