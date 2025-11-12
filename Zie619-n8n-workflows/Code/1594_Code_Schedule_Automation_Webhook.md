# Workflow Analysis for Matomo Analytics Report

## Description
This workflow automatically retrieves visitor data from Matomo Analytics for users who have visited the site more than 3 times in the last 30 days, sends it to an AI (LLaMA) for SEO analysis, and stores the AI-generated insights in a Baserow database.

## Input Details
The workflow is triggered either manually or on a weekly schedule and receives no external input data—it pulls data directly from the Matomo API using predefined parameters.

## Process Summary
The workflow starts with a manual or scheduled trigger. It then fetches detailed visitor data from Matomo for repeat visitors over the last 30 days. A code node formats this data into a structured prompt highlighting visitor behavior. This prompt is sent to an AI model via an HTTP request for SEO analysis. Finally, the AI's response is saved to a Baserow table with the current date, the insight content, and the blog name.

## Output Details
The workflow stores AI-generated SEO insights in a Baserow database table with fields for date, note (insights), and blog name.

## Tags
Matomo, SEO, AI analysis, analytics, automation, Baserow, LLaMA, scheduled report, visitor insights, n8n
