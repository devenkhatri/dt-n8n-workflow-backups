# Workflow Analysis for Learn Something Every Day - Scheduled Factoid Email Service

## Description
This workflow powers an automated email subscription service that sends daily, weekly, or surprise factoids on topics chosen by users. It handles user subscriptions and unsubscribes via web forms, stores subscriber data in Airtable, and uses AI to generate personalized content and images for each email.

## Input Details
The workflow is triggered by three sources: a daily schedule at 9 AM, a subscription form submission, and an unsubscribe form submission.

## Process Summary
When a user subscribes via the form, their details are saved to Airtable and a confirmation email is sent. The daily schedule trigger fetches active subscribers based on their frequency preference (daily, weekly with last-sent check, or random 'surprise' selection). Each qualifying subscriber is processed in a subworkflow that generates a unique factoid and matching image using AI, formats an HTML email with an unsubscribe link, sends it via Gmail, and logs the send time back to Airtable. Unsubscribe requests deactivate the subscriber in Airtable using their unique ID.

## Output Details
The workflow sends personalized factoid emails to subscribers with generated text and images, logs send timestamps in Airtable, and deactivates subscriptions upon request.

## Tags
email automation, subscription service, scheduled workflow, Airtable integration, AI content generation, form handling, Gmail integration, n8n workflow
