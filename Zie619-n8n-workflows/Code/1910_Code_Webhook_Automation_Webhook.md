# Workflow Analysis for Lead Qualification with BatchData

## Description
This workflow automatically qualifies new sales leads by verifying and enriching their property information using BatchData's API, assigning a lead score based on property characteristics, updating the CRM with the enriched data, and triggering immediate follow-up actions for high-value leads.

## Input Details
The workflow is triggered by a webhook when a new lead is created in the CRM, receiving the lead ID and address details (address, city, state, ZIP code).

## Process Summary
First, the workflow receives a new lead via a CRM webhook. It then fetches complete lead data from the CRM API. Next, it queries the BatchData API to verify and enrich the lead with detailed property information. A custom scoring function evaluates the property data and assigns a qualification status (e.g., high-value, qualified, potential). Finally, the workflow updates the CRM with the score, status, and property details.

## Output Details
The workflow updates the CRM lead record with qualification data and, for high-value leads, creates an urgent follow-up task in the CRM and sends a Slack notification to the sales team.

## Tags
lead qualification, CRM integration, property data, BatchData API, lead scoring, automation, sales follow-up, Slack notification
