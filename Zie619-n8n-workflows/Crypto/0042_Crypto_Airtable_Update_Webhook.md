# Workflow Analysis for URL Shortener with Analytics Dashboard

## Description
This workflow implements a custom URL shortening service with tracking and a live analytics dashboard. It generates shortened URLs from long ones, stores them with click statistics in Airtable, redirects users when they visit a short link, and provides a web dashboard showing total clicks, links, and unique domains.

## Input Details
The workflow is triggered by three webhooks: one to create short URLs (with a 'url' query parameter), one to redirect users (with an 'id' query parameter), and one to view the analytics dashboard.

## Process Summary
When a long URL is submitted, it's validated, hashed using SHA256, and a 6-character ID is extracted to create a short URL. The system checks if this ID already exists in Airtable to avoid duplicates. If not, it stores the short URL, long URL, ID, host, and initializes click count. When a short URL is accessed, the system looks up the ID in Airtable, redirects the user to the original URL, and increments the click counter. The dashboard webhook fetches all stored links, calculates total clicks, total links, and unique hosts, then renders an HTML page with these stats.

## Output Details
The workflow returns a short URL when creating one, redirects users to the original URL when accessing a short link (while updating click counts), and serves an HTML analytics dashboard showing usage statistics.

## Tags
url shortener, link shortener, analytics dashboard, airtable integration, webhook, redirect service, click tracking, n8n workflow
