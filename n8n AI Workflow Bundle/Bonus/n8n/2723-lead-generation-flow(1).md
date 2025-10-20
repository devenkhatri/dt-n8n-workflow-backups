# Workflow Analysis for Automated Lead Generation and Outreach Workflow

## Description
This workflow automates the process of generating leads from social media posts, enriching them with publicly available data, filtering them based on specific criteria, and then initiating personalized outreach via email.

## Input Details
The workflow is triggered by new posts on Reddit that match specified search terms (e.g., "AI workflow" and "n8n").

## Process Summary
The workflow starts by fetching new Reddit posts containing "AI workflow" and "n8n", then extracts the author and permalink of each post. Next, it uses the "Phantombuster Phantom" node to extract public profile data of the authors. A "Switch" node then checks the follower count; if an author has more than 50, a custom prompt is used to generate a personalized outreach email, otherwise a generic email is crafted. Finally, the workflow sends the generated email via SendGrid.

## Output Details
The workflow sends personalized outreach emails to potential leads via SendGrid.
