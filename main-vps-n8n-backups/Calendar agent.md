# Workflow Analysis for Calendar Event Creation and Notification

## Description
This workflow automates the creation of calendar events and sends notifications using a large language model to process event details from a webhook.

## Input Details
The workflow is triggered by an HTTP webhook that receives event details as input.

## Process Summary
The workflow starts by extracting and transforming data from the incoming webhook. It then uses the OpenAI Chat Completions node to process the event details using a specified AI model and temperature. The processed information is then used to create a new calendar event in Google Calendar. Finally, a notification is sent via Telegram to a designated chat ID, informing about the newly created event.

## Output Details
The workflow creates a Google Calendar event and sends a Telegram notification.
