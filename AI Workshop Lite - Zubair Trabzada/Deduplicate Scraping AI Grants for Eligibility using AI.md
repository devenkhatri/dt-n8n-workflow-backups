# Workflow Analysis for Daily AI Grant Opportunity Digest with Eligibility Check

## Description
This workflow automates the process of finding new AI grant opportunities, assessing their eligibility using AI, tracking them in Airtable, and sending a daily email digest to relevant stakeholders.

## Input Details
The workflow is triggered by two daily schedules; one fetches recent AI grant opportunities from Grants.gov, and the other retrieves newly processed eligible grants from Airtable.

## Process Summary
The workflow first fetches recent "AI" grant opportunities from Grants.gov daily and filters out any duplicates already processed. For each new grant, it retrieves detailed information and then uses AI (OpenAI) to summarize the grant's synopsis and determine eligibility based on predefined company information. The summarized and analyzed grant details are then saved into an Airtable database. Later in the day, the workflow searches the Airtable for newly added and eligible grants from that day. It then generates an HTML email summarizing these eligible grants and retrieves a list of active email subscribers from Airtable, finally sending the personalized email digest to each active subscriber via Gmail.

## Output Details
The workflow stores new, analyzed grant opportunities in an Airtable database and sends a daily HTML email alert containing a summary of eligible grants to a list of subscribers.
