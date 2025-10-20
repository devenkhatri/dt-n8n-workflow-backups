# Workflow Analysis for Webflow Form Submission to Discord Notification

## Description
This workflow processes submissions from a Webflow form, extracts relevant data, and sends a formatted notification to a Discord channel.

## Input Details
The workflow is triggered by an incoming webhook from a Webflow form submission, receiving data such as name, email, and message.

## Process Summary
The workflow starts by catching a webhook from a Webflow form. It then extracts the specific fields like name, email, and message from the form data using an "Item Lists" node. A "Set" node then structures this extracted information into a clear, readable message. Finally, an "If" node checks if the message is valid, and if so, it proceeds to send the formatted message to a designated Discord channel.

## Output Details
The workflow sends a formatted notification containing the form submission details to a specified Discord channel.
