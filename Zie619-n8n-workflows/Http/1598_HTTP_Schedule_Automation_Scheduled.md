# Workflow Analysis for AirQuality Scheduler

## Description
This workflow automatically fetches real-time air quality and pollen data, combines it with a user's health profile, and uses an AI to generate personalized environmental health summaries and suggestions, then sends these as an email.

## Input Details
The workflow is triggered daily at 7 AM and uses predefined location coordinates, age, and health sensitivities as input for fetching data and generating personalized advice.

## Process Summary
1. The workflow is initiated daily at 7 AM by a schedule trigger.
2. It sets predefined latitude and longitude for a location and a user profile including age and health sensitivities.
3. It fetches current air quality and pollen data from an external API using the specified location coordinates.
4. An AI agent then processes this environmental data along with the user's profile to create a friendly summary of conditions and provide practical, personalized health suggestions.
5. The AI's generated message, containing the summary and suggestions, is then prepared to be sent via email.

## Output Details
The workflow generates a personalized environmental health summary and tailored suggestions, which are delivered to a specified email address via Gmail.

## Tags
automation, n8n, production-ready, excellent, optimized, Air Quality, Pollen, Environmental Health, Scheduler, AI, Gmail, Notifications
