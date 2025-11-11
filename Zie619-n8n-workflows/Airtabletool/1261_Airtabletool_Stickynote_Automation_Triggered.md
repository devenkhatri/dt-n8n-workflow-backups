# Workflow Analysis for AI Social Media Caption Creator

## Description
This workflow automatically generates engaging, audience-tailored social media captions using AI. It pulls briefing details and audience background information from Airtable, crafts a creative caption with a call-to-action, and writes the result back to the original Airtable record.

## Input Details
The workflow is triggered when a new record is created in a specific Airtable table, and it receives the record's briefing notes and other metadata.

## Process Summary
The workflow starts by monitoring an Airtable table for new records. After a 1-minute wait to allow data entry, it fetches the full record data. An AI agent then uses this briefing along with audience and tonality details retrieved from another Airtable table to generate a tailored social media caption. The resulting caption is formatted and updated in the original Airtable record under the 'SoMe_Text_KI' field.

## Output Details
The workflow outputs a polished social media caption and updates it directly in the corresponding Airtable record.

## Tags
AI, social media, caption generation, Airtable, automation, n8n, content creation, Instagram, GPT-4, marketing
