# Workflow Analysis for Learn Something Every Day - Automated Factoid Email Service

## Description
This workflow provides a fully automated email subscription service that sends daily, weekly, or surprise factoids on user-selected topics. Subscribers can sign up or unsubscribe via web forms, and the system uses AI to generate unique content and images for each email.

## Input Details
The workflow is triggered by three sources: a scheduled trigger running daily at 9 AM, a subscription form submission, and an unsubscribe form submission.

## Process Summary
When a user subscribes via the form, their details are saved to Airtable and a confirmation email is sent. The daily scheduled trigger searches for active subscribers based on their frequency (daily, weekly, or surprise) and processes them. Weekly subscribers are only processed if their last email was sent more than 7 days ago, while surprise subscribers are randomly selected. For each selected subscriber, the workflow executes a subworkflow that uses an AI agent with Wikipedia access to generate a unique factoid on their chosen topic, creates a complementary image, resizes it, and sends both in a personalized HTML email with an unsubscribe link. After sending, the 'Last Sent' date is updated in Airtable.

## Output Details
The workflow sends personalized HTML emails containing AI-generated factoids and images to subscribers, updates subscriber records in Airtable with the last sent timestamp, and deactivates subscriptions when users unsubscribe.

## Tags
email automation, subscription service, AI content generation, scheduled workflows, Airtable integration, form processing, Gmail, Wikipedia API, image generation, unsubscribe management
