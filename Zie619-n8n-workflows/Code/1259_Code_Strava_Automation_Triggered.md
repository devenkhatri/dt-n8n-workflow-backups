# Workflow Analysis for Strava Activity Analysis and Coaching Workflow

## Description
This workflow automatically analyzes new or updated Strava activities and provides personalized coaching feedback as if from a professional triathlon coach. It processes activity data, generates actionable insights using AI, formats the response in HTML, and delivers it via email and WhatsApp.

## Input Details
The workflow is triggered by a Strava webhook whenever an activity is created or updated, receiving detailed activity data in JSON format.

## Process Summary
The workflow starts by receiving Strava activity data via a webhook. It then flattens and combines the JSON data into a readable string format. This formatted data is passed to a Google Gemini AI model with a custom prompt that simulates a triathlon coach analyzing the activity. The AI returns structured coaching advice, which is then parsed, converted into HTML, and sent via both email and WhatsApp to the user.

## Output Details
The workflow produces a personalized, HTML-formatted coaching analysis of the Strava activity and sends it via email and WhatsApp to the user.

## Tags
Strava, AI coaching, triathlon, fitness, Google Gemini, automation, email notification, WhatsApp, workout analysis, n8n
