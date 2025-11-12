# Workflow Analysis for Price Tracker with Email Alerts

## Description
This workflow automatically monitors product prices on specified websites every 15 minutes. It checks if prices have dropped compared to previously recorded values and sends an email notification when a better price is found. It also alerts the user if it fails to extract a valid price from a webpage.

## Input Details
The workflow is triggered every 15 minutes by a cron scheduler and uses a hardcoded list of product URLs, CSS selectors, and currencies defined in the 'changeME' function node.

## Process Summary
The workflow loops through a list of product items, fetching each product's webpage and extracting the price using a CSS selector. It compares the current price with the previously saved price (stored in a JSON file). If the price has decreased, it updates the saved data and sends an email alert. If no valid price is found, it sends a troubleshooting email. The workflow handles both initial setup (when no price file exists) and ongoing monitoring.

## Output Details
The workflow saves updated product price data to a local JSON file and sends email notifications for price drops or extraction errors.

## Tags
price tracking, email alerts, web scraping, automation, cron job, product monitoring, n8n
