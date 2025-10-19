# Workflow Analysis for Email Triage Agent with Gmail

## Description
This workflow automates the triaging of incoming emails using AI to categorize them and then take appropriate actions like moving them to specific folders or sending replies.

## Input Details
The workflow is triggered manually and receives no direct input data upon initiation.

## Process Summary
The workflow first retrieves unread emails from a specified Gmail inbox. Then, it uses an AI model to classify each email based on its content, determining if it is generic, a sales inquiry, or a support request. Based on the classification, the workflow either moves the email to a designated folder (Sales or Support) or, for generic emails, marks them as read. Additionally, if an email is classified as a sales or support inquiry, the workflow composes and sends a relevant automated reply.

## Output Details
The workflow moves emails to specific Gmail folders, marks emails as read, and sends automated email replies.
