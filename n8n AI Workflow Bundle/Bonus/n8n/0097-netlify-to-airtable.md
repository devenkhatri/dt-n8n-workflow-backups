# Workflow Analysis for Netlify to Airtable Submission

## Description
This workflow captures new form submissions from Netlify and automatically saves them as new records in a specified Airtable base. This automation helps streamline lead capture or data collection processes.

## Input Details
The workflow is triggered by an HTTP POST request, typically from a Netlify form submission webhook, receiving form submission data.

## Process Summary
The workflow starts by receiving submission data from Netlify. It then extracts the form fields from the incoming data. Finally, it creates a new record in Airtable using the extracted form fields.

## Output Details
The workflow creates a new record in a specified Airtable base, storing the Netlify form submission data.
