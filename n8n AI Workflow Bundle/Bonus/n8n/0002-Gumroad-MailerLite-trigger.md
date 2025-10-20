# Workflow Analysis for Gumroad to MailerLite Subscriber Automation

## Description
This workflow automates the process of adding new Gumroad customers to a MailerLite subscriber list, ensuring that every purchase automatically updates your email marketing platform.

## Input Details
This workflow is triggered by new sales events from Gumroad via a webhook.

## Process Summary
The workflow starts with a webhook listening for Gumroad sales. It then checks if an email address is provided in the Gumroad data. If the email exists, the workflow extracts the customer's name and email. Finally, it uses this information to add or update the subscriber in a specified MailerLite group.

## Output Details
The workflow adds or updates subscriber information (name, email) in a MailerLite group.
