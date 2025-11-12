# Workflow Analysis for Luma AI - Webhook Response v1 - AK

## Description
This workflow automatically processes webhook responses from Luma AI containing generated video and thumbnail URLs, then updates the corresponding record in an Airtable base with the new media links and marks it as 'Done'.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing a JSON payload from Luma AI with video generation results.

## Process Summary
The workflow starts by receiving a webhook payload from Luma AI. It extracts the video URL, thumbnail URL, and generation ID from the payload. It then checks if the video URL is present. If so, it prepares global settings including Airtable base and table IDs, and updates the corresponding Airtable record using the generation ID as a match key, setting the status to 'Done' and adding the video and thumbnail URLs.

## Output Details
The workflow updates a record in a specified Airtable table by adding the video and thumbnail URLs and changing the status to 'Done'.

## Tags
Luma AI, webhook, Airtable, video generation, automation, n8n, production-ready
