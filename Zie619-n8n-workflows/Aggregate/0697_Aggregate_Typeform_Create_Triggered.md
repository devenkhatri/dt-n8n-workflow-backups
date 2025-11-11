# Workflow Analysis for Set Workflow

## Description
This workflow automatically processes quiz responses submitted via Typeform, transforms the data into a KlickTipp-compatible format, and adds the respondent as a subscriber in KlickTipp with relevant tags based on their answers.

## Input Details
The workflow is triggered by a new quiz submission from a Typeform form, receiving user-provided data such as name, email, phone number, birthday, and quiz answers.

## Process Summary
First, the workflow captures a new Typeform quiz submission. It then formats key fields like phone number (to numeric-only with '00' prefix), birthday (to UNIX timestamp), and quiz answers (to comma-separated strings or scaled numbers). Next, it checks which tags derived from quiz answers already exist in KlickTipp by fetching all existing tags and comparing them. For any non-existent tags, it creates them in KlickTipp. Finally, it tags the new subscriber with both existing and newly created tags.

## Output Details
The workflow adds the quiz respondent as a new subscriber in KlickTipp with mapped personal data and applies dynamic tags based on their quiz responses, enabling automated follow-up campaigns.

## Tags
Typeform, KlickTipp, lead generation, contact tagging, data transformation, automation, quiz processing, subscriber management, tag creation, production-ready
