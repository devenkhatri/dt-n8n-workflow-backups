# Workflow Analysis for AI Meeting Assistant: Pre-Meeting WhatsApp Notifications

## Description
This workflow acts as an AI-powered meeting assistant, generating and sending concise pre-meeting notifications to a user's WhatsApp. It helps busy professionals quickly get up to speed on upcoming meetings by providing relevant context about attendees.

## Input Details
The workflow is triggered hourly by a scheduled event and receives upcoming Google Calendar meeting details scheduled within the next hour.

## Process Summary
The workflow first retrieves upcoming Google Calendar meetings and extracts attendee information using an OpenAI model. For each attendee, it attempts to find and summarize their last email correspondence via Gmail and scrapes their LinkedIn profile for recent activity using Apify.com, then summarizes this information with an OpenAI model. It then aggregates all attendee data with their respective summaries. An OpenAI model generates a tailored pre-meeting notification, incorporating meeting details and attendee insights.

## Output Details
The workflow sends a comprehensive pre-meeting notification as a WhatsApp message to the user.
