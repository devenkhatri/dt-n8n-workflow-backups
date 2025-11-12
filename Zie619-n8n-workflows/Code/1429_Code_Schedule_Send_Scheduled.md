# Workflow Analysis for Learn Something Every Day - Scheduled Factoid Email Service

## Description
This workflow automates a subscription-based email service that sends daily, weekly, or surprise factoids on topics chosen by users. It handles subscriptions, unsubscriptions, content generation using AI, and scheduled email delivery with proper tracking.

## Input Details
The workflow is triggered by three sources: a scheduled trigger running daily at 9 AM, a subscription form submission, and an unsubscription form submission.

## Process Summary
The workflow manages user subscriptions via a form and stores subscriber data in Airtable. A daily schedule triggers searches for active subscribers based on their chosen frequency (daily, weekly, or surprise). For weekly subscribers, it checks if 7 days have passed since the last email. Surprise emails are sent randomly (1 in 10 chance). Selected subscribers are processed in subworkflows where AI generates personalized factoids and complementary images. The system then emails the content to subscribers and logs the send time in Airtable. Unsubscription requests deactivate a user's subscription using a unique ID.

## Output Details
The workflow sends personalized factoid emails with images to subscribers, updates Airtable with the last sent timestamp, and deactivates subscriptions when requested via the unsubscribe form.

## Tags
email automation, subscription service, AI content generation, scheduled workflow, Airtable integration, form handling, Gmail integration
