# Workflow Analysis for Bitrix24 Task Form Widget Application Workflow example with Webhook Integration

## Description
This workflow handles the installation and operation of a custom Bitrix24 task form widget. It securely captures and stores authentication credentials during app installation, and later retrieves and displays detailed task data when the widget is opened in a Bitrix24 task view.

## Input Details
The workflow is triggered by HTTP POST requests from Bitrix24 containing either installation data (event=ONAPPINSTALL or PLACEMENT=DEFAULT) or widget placement requests with task context.

## Process Summary
The workflow first extracts authentication and domain data from the incoming webhook request. It checks if the request is for app installation or widget display. During installation, it saves credentials to a settings file and registers the widget placement in Bitrix24. For widget display requests, it reads the saved settings, fetches the specific Bitrix24 task data using the task ID from the request, formats it as an HTML table, and returns it to be shown in the widget.

## Output Details
The workflow responds with HTML pages: an installation completion page during setup, a formatted task data table when the widget is viewed, or an error page if settings are missing or invalid.

## Tags
bitrix24, widget, task management, webhook, installation, integration, automation, n8n, production-ready
