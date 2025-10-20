# Workflow Analysis for Strava Coaching Workflow

## Description
This workflow automates the process of fetching Strava activities, generating a coaching summary using AI, and sending this summary via email.

## Input Details
The workflow is manually triggered or can be scheduled to run at specific intervals.

## Process Summary
The workflow starts by fetching recent activities from Strava for a specified athlete. It then formats the activity data into a readable array. Next, it uses OpenAI to generate a coaching summary based on these activities. Finally, it formats the summary into an HTML email.

## Output Details
The workflow sends an email containing the AI-generated coaching summary.
