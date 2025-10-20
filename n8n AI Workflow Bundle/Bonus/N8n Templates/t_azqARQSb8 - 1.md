# Workflow Analysis for Webflow Form Submission to Discord Notification

## Description
This workflow automatically sends a notification to a Discord channel whenever a new form is submitted on your Webflow site.

## Input Details
The workflow is triggered by an incoming webhook from a Webflow form submission, receiving data about the submitted form fields.

## Process Summary
The workflow starts by receiving data from a Webflow form submission via a webhook. It then converts this data into a formatted JSON string. Next, it constructs a message that includes the Webflow form ID and the stringified form data. Finally, it sends this message as a notification to a specified Discord channel.

## Output Details
The workflow sends a message containing Webflow form submission details to a Discord channel.
