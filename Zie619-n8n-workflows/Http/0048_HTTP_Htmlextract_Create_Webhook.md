# Workflow Analysis for Production Workflow

## Description
This workflow automatically processes incoming webhook requests containing a URL. If the request type is not 1, it fetches the webpage, extracts its title, saves the title and URL to a Notion database, and sends a confirmation reply to Discord. If the type is 1, it simply registers the URL by setting the type to 1.

## Input Details
The workflow is triggered by a POST request to a unique webhook URL, receiving a JSON payload that includes a 'type' field and a URL via the environment variable BASE_URL.

## Process Summary
The workflow starts with a webhook trigger that receives a payload. It checks if the 'type' field in the payload is not equal to 1. If true, it makes an HTTP request to the URL in the BASE_URL environment variable, extracts the webpage's title using HTML extraction, and adds both the title and URL to a specified Notion database. It then prepares a success reply for Discord. If the 'type' is 1, it bypasses processing and just sets the type to 1. Any errors during execution are handled by an error handler node that stops the workflow with an error message.

## Output Details
The workflow either adds a new page to a Notion database with the webpage title and URL and returns a success message formatted for Discord, or it returns a minimal response indicating the URL was registered (type 1).

## Tags
webhook, notion, discord, html extraction, automation, production, error handling
