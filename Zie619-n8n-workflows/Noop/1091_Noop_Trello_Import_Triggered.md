# Workflow Analysis for Get Product Feedback

## Description
This workflow automates the collection and management of product feedback by capturing responses from a Typeform survey, storing them in Airtable, and creating a Trello card for high-scoring feedback to facilitate further action.

## Input Details
The workflow is triggered by new submissions to a Typeform survey, receiving product feedback data including a score, name, email, and description.

## Process Summary
1. The workflow starts when a user submits a Typeform survey.
2. It then extracts the submitted product feedback details, including the score, name, email, and a description.
3. This feedback data is appended as a new record to the "Feedback" table in Airtable.
4. Next, the workflow checks if the submitted feedback score is greater than 7.
5. If the score is greater than 7, a new card is created in Trello with the detailed feedback; otherwise, no further action is taken in this branch.

## Output Details
The workflow outputs feedback entries to an Airtable database and, for positive feedback (score > 7), creates a corresponding card in Trello for further processing.

## Tags
automation, n8n, production-ready, excellent, optimized, Typeform, Airtable, Trello, Feedback, Survey
