# Workflow Analysis for Website check

## Description
This workflow periodically checks a website's content to see if it contains the phrase 'Out Of Stock' and sends a notification to Discord depending on whether the phrase is found or not.

## Input Details
The workflow is triggered on an hourly schedule via a Cron node and fetches data from a specified website URL using an HTTP request.

## Process Summary
The workflow starts by making an HTTP request to a configured website URL. It then checks if the response data contains the phrase 'Out Of Stock'. If the phrase is found, it sends a 'value found' message to a Discord webhook; otherwise, it sends a 'value not found' message. The workflow includes error handling to manage any failures during execution.

## Output Details
The workflow sends one of two messages to a Discord channel via a webhook depending on whether the target phrase is detected on the website.

## Tags
website monitoring, stock checker, Discord alert, cron job, HTTP request, conditional logic, error handling
