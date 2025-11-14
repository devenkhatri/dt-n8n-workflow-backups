# Workflow Analysis for Track Working Time and Pauses

## Description
This automated workflow integrates with an iOS Shortcut to manage daily work time and pauses. It uses Notion as a backend to record start times, break durations, and end times, providing a simple time tracking solution.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint, receiving JSON data that includes a "method" (start, break, or end) and optionally a "duration" for breaks.

## Process Summary
The workflow begins by receiving a request from an iOS Shortcut. It then uses a Switch node to direct the flow based on the "method" provided in the input, which can be "start", "break", or "end". For "start" and "end" methods, it retrieves the Notion page for the current day and either creates a new entry (for "start") or updates the existing entry with the end time. For the "break" method, it captures the break duration and updates the Notion page with this information. Throughout the process, it sets various messages indicating the status or outcome of each operation.

## Output Details
The workflow updates a designated Notion database ("Time Tracker") by creating new pages or modifying existing ones with start times, end times, and break durations, and returns a text message response to the triggering iOS Shortcut.

## Tags
automation, n8n, production-ready, excellent, optimized, Notion, Time Tracking, API, Webhook
