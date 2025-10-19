# Workflow Analysis for AI-powered Bug Classification in Linear

## Description
This workflow automates the classification of new bugs reported in Linear using OpenAI's GPT-4 and then assigns them to the appropriate team based on the classification.

## Input Details
The workflow is triggered by new "Bug" issues created in Linear.

## Process Summary
The workflow starts when a new bug is reported in Linear. It then uses OpenAI's GPT-4 to categorize the bug based on its title and description. A Switch node directs the bug to the correct team based on the GPT-4 classification (e.g., Frontend, Backend, API, Mobile). Finally, the Linear issue is updated to assign it to the identified team.

## Output Details
The workflow updates the Linear issue, assigning the newly created bug to the correct team.
