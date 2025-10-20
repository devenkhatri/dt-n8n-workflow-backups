# Workflow Analysis for HubSpot Contact Summarizer with ChatGPT

## Description
This workflow automates the summarization of HubSpot contact notes using ChatGPT upon an update in HubSpot. The summarized notes are then added back to the HubSpot contact, enhancing efficiency in managing customer interactions.

## Input Details
The workflow is triggered by updates to contact properties in HubSpot via a webhook.

## Process Summary
The workflow starts by retrieving the updated contact from HubSpot. It then filters the contact updates to proceed only if the "notes_activities" property has changed. Next, all notes associated with the contact are fetched from HubSpot. These notes are then compiled and sent to ChatGPT to generate a concise summary. Finally, the generated summary is added as a new note to the corresponding contact in HubSpot.

## Output Details
The workflow outputs a summarized note, which is then added as a new note to the HubSpot contact that triggered the workflow.
