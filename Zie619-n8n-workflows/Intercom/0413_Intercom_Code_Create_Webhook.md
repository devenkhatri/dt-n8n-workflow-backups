# Workflow Analysis for Enrich Intercom Users with ExactBuyer Data

## Description
This workflow automates the enrichment of new contacts in Intercom by fetching detailed contact information from ExactBuyer. It updates Intercom user profiles with social profiles, contact data (phone, email), and location details, making the Intercom profiles more comprehensive and useful.

## Input Details
The workflow is triggered by an Intercom webhook event, specifically when a new user contact is created.

## Process Summary
1. The workflow starts upon receiving a "contact.user.created" webhook event from Intercom. 2. It then extracts the user's ID and email from the incoming webhook data. 3. Next, it queries the ExactBuyer API using the extracted email to retrieve enriched user information. 4. The retrieved data is then massaged into a suitable format, specifically structuring social profiles and location data. 5. Finally, the workflow updates the user's profile in Intercom with the enriched details including updated email, name, phone, avatar, social profiles, and location.

## Output Details
The workflow updates an existing user's profile in Intercom with enriched contact details from ExactBuyer.

## Tags
Intercom, ExactBuyer, user enrichment, CRM, automation, webhook, contact management
