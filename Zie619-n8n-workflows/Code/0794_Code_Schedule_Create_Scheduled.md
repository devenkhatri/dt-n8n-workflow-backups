# Workflow Analysis for Invite Users to n8n from Google Sheets

## Description
This workflow automates the process of inviting new users to an n8n instance by comparing email addresses from a Google Sheet against existing users in n8n. Only non-existing users are invited via an API call, and the workflow supports both manual and scheduled execution.

## Input Details
The workflow is triggered either manually by clicking 'Test workflow' or automatically via a schedule, and it pulls user data from a specified Google Sheet and an external API endpoint for existing n8n users.

## Process Summary
The workflow first retrieves all existing users from the n8n API with pagination support, then fetches all rows from a designated Google Sheet containing email addresses. It compares the two datasets to identify email addresses in the sheet that don’t already exist as users. For each new email, it formats a user object with a default role and sends an invitation via a POST request to the n8n API.

## Output Details
The workflow sends API requests to create new user accounts in n8n for previously unregistered email addresses from the Google Sheet, triggering invitation emails to those users.

## Tags
user provisioning, Google Sheets, n8n API, automation, scheduled workflow, user onboarding, email invitation
