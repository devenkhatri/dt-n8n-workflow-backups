# Workflow Analysis for AI Social Media Caption Creator

## Description
This workflow automatically generates engaging, audience-tailored social media captions using AI, based on a briefing and background information stored in Airtable. The generated caption is then saved back to the corresponding Airtable record.

## Input Details
The workflow is triggered by a new record in a specific Airtable table, and it receives the record’s 'Briefing/Notizen' field as input after a short delay to allow for data entry.

## Process Summary
The workflow starts when a new record is added to an Airtable editorial planning table. After waiting one minute to ensure the briefing is fully entered, it retrieves the record data. An AI agent, powered by OpenAI's GPT-4o, uses the briefing and fetches additional background context (like target audience and tone) from another Airtable table. The AI then generates a creative, on-brand caption with a call-to-action. Finally, the caption is formatted and written back to the original Airtable record in the 'SoMe_Text_KI' field.

## Output Details
The workflow outputs an AI-generated social media caption and updates the corresponding Airtable record with this caption in the 'SoMe_Text_KI' field.

## Tags
AI, social media, caption generation, Airtable, automation, n8n, content creation, OpenAI, workflow, editorial planning
