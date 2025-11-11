# Workflow Analysis for Strava Activity Coaching Workflow

## Description
This workflow automatically analyzes new or updated Strava activities using an AI-powered triathlon coach, then delivers personalized, motivational performance feedback via email and WhatsApp.

## Input Details
The workflow is triggered by an update to a Strava activity (e.g., after a run, swim, or bike ride is saved or edited).

## Process Summary
When a new Strava activity is recorded or updated, the workflow captures the raw activity data. It then flattens and combines all JSON fields into a readable string format. This data is passed to a Google Gemini AI model that acts as a triathlon coach, using a detailed prompt to generate personalized, sport-specific feedback and improvement suggestions. The AI’s plain-text response is parsed, structured into headings, paragraphs, and lists, then converted into HTML for rich formatting. Finally, the formatted coaching insights are sent via email and WhatsApp.

## Output Details
The workflow sends a personalized HTML-formatted coaching analysis of the Strava activity to both an email address and a WhatsApp number.

## Tags
Strava, fitness coaching, AI analysis, Google Gemini, email automation, WhatsApp automation, triathlon, workout feedback, n8n, automation
