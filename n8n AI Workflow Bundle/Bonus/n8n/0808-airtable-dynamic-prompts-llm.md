# Workflow Analysis for Airtable Dynamic Prompts with LLM

## Description
This workflow retrieves dynamic prompts from Airtable, processes them using a large language model, and updates a Google Sheet and Airtable with the generated content.

## Input Details
This workflow is triggered manually.

## Process Summary
The workflow starts by fetching data from an Airtable base containing prompts. It then iterates through each prompt, uses a large language model to generate content based on the prompt, and stores the generated content. Finally, it updates a Google Sheet with the prompt and generated content, and updates the original Airtable record with the generated content.

## Output Details
The workflow outputs updated records in Google Sheets and Airtable, containing the generated content from the large language model.
