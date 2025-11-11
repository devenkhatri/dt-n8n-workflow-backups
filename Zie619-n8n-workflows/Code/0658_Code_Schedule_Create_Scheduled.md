# Workflow Analysis for Learn Something Every Day - Scheduled Factoid Email Service

## Description
This workflow automates a subscription-based email service that sends users interesting facts on topics they choose, either daily, weekly, or as a surprise. It manages subscriptions, generates AI-powered content and images, sends personalized emails, and handles unsubscriptions—all while tracking delivery status in Airtable.

## Input Details
The workflow is triggered by three sources: a daily schedule (at 9 AM UTC), a subscription form submission, and an unsubscription form submission.

## Process Summary
First, users subscribe via a form, which saves their email, topic, and frequency preference to Airtable and sends a confirmation email. Separately, every day at 9 AM, the workflow checks Airtable for active subscribers based on their frequency (daily, weekly, or surprise). Weekly emails are only sent if the last email was over 7 days ago, and surprise emails are sent randomly (10% chance). For each qualifying subscriber, the workflow executes a subworkflow that uses AI to generate a unique factoid and a complementary image, then emails it to the user with an unsubscribe link. Finally, it logs the send time back to Airtable. Unsubscribe requests deactivate the user’s record using their unique ID.

## Output Details
The workflow sends personalized AI-generated factoid emails with images to subscribers, logs send timestamps in Airtable, and updates subscriber status upon unsubscription.

## Tags
email automation, subscription service, Airtable integration, AI content generation, scheduled workflow, form handling, Gmail, n8n workflow, daily facts, unsubscription management
