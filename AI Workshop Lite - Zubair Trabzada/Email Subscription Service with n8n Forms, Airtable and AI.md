# Workflow Analysis for Learn Something Every Day - Automated Factoid Email Service

## Description
This workflow provides a complete automated email subscription service that sends daily, weekly, or surprise factoids about user-requested topics. Subscribers can sign up through a web form and later unsubscribe using a unique ID. The system uses AI to generate unique factoids and accompanying images, then emails them according to the subscriber's chosen frequency.

## Input Details
The workflow is triggered by three sources: a daily scheduled trigger at 9 AM, a subscription form submission, and an unsubscribe form submission.

## Process Summary
When users subscribe via the form, their details are saved to Airtable and a confirmation email is sent. The daily schedule trigger searches for active subscribers by frequency type (daily, weekly, or surprise), with weekly subscribers only processed if their last email was sent more than 7 days ago. For surprise subscribers, a random chance (10%) determines if they receive an email. Selected subscribers are processed through a subworkflow that uses an AI agent with Wikipedia access to generate a unique factoid about their topic, creates a complementary image, resizes it, and sends both in an HTML email with an unsubscribe link. After sending, the subscriber's 'Last Sent' date is updated in Airtable.

## Output Details
The workflow sends personalized HTML emails containing AI-generated factoids and images to subscribers, updates subscriber records in Airtable with the last sent timestamp, and processes unsubscriptions by marking records as inactive.

## Tags
email automation, subscription service, AI content generation, scheduled workflow, Airtable integration, form handling, Gmail integration, LangChain, Groq, OpenAI
