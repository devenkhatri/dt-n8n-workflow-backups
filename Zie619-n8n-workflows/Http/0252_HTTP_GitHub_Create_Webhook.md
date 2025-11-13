# Workflow Analysis for GitHub Fork to Pipedrive Lead Automation

## Description
This workflow automatically captures GitHub repository fork events, retrieves the forker's details, and creates a lead in Pipedrive CRM. If the user doesn’t already exist in Pipedrive, it creates a new person record before creating the lead, and adds a note with the user’s GitHub profile URL.

## Input Details
The workflow is triggered by a GitHub 'fork' webhook event for the repository 'DemoRepo' owned by 'John-n8n'.

## Process Summary
The workflow starts when a GitHub fork event occurs. It fetches the forker’s GitHub user information via an HTTP request, then searches Pipedrive for an existing person using the user's email. If a person is found, it proceeds to create a lead linked to that person. If not, it creates a new person in Pipedrive using the GitHub username and email, then creates the lead. Finally, it adds a note to the lead with the forker's GitHub profile URL.

## Output Details
The workflow creates a new lead in Pipedrive associated with a person (either existing or newly created) and attaches a note containing the GitHub user’s profile URL.

## Tags
GitHub, Pipedrive, CRM, automation, lead generation, fork event, webhook, integration
