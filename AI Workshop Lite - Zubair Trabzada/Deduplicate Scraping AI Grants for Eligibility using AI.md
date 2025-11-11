# Workflow Analysis for AI Grant Opportunity Tracker and Alert System

## Description
This workflow automatically discovers new AI-related grant opportunities from grants.gov, uses AI to assess eligibility and summarize key details, stores qualified grants in Airtable, and sends a daily email digest to subscribers with relevant opportunities.

## Input Details
The workflow is triggered twice daily by scheduled triggers—at 8:30 AM to fetch new AI-related grants from grants.gov posted in the last 24 hours, and at 9:00 AM to retrieve newly added eligible grants from Airtable for email distribution.

## Process Summary
First, the workflow fetches AI-related grant listings from grants.gov and filters out any previously processed grants using a deduplication node. For each new grant, it retrieves full details via an API call. Two AI models then analyze the grant: one summarizes the goal, duration, success criteria, and key notes, while the other evaluates eligibility based on the organization’s profile. The results are merged and saved to an Airtable base with structured fields. Later, the workflow queries Airtable for all newly added eligible grants from the current day, formats them into an HTML email newsletter, and sends it to active subscribers from a separate Airtable subscribers list.

## Output Details
The workflow saves processed grant data to an Airtable base and sends a daily HTML-formatted email newsletter with new eligible AI grant opportunities to a list of subscribers via Gmail.

## Tags
grants, AI, eligibility screening, automation, Airtable, email alert, government funding, n8n workflow, OpenAI, grants.gov
