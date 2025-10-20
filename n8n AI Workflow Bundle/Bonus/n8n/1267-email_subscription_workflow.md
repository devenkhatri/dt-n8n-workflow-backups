# Workflow Analysis for Email Subscription Workflow

## Description
This workflow manages email subscriptions by capturing form submissions, validating email addresses, and performing actions based on subscription status.

## Input Details
The workflow is triggered by an n8n form submission, receiving email addresses and other form data.

## Process Summary
The workflow starts by extracting the email from the form data and validating its format. It then checks if the email is already in the "Subscribed" Mailchimp list. If subscribed, it sends a thank you email and does nothing further. If unsubscribed, it adds the email to the "Active" Mailchimp list and moves it out of the "Unsubscribed" list. If the email is not found, it adds it to the "Subscribed" Mailchimp list. Finally, it sends an email confirmation.

## Output Details
The workflow updates Mailchimp lists and sends email confirmations or thank you messages via SendGrid.
