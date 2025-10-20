# Workflow Analysis for Slack to Linear Ticket Creation

## Description
This workflow automates the creation of Linear tickets from specific Slack messages, extracting key information to streamline issue tracking and project management.

## Input Details
The workflow is triggered manually and receives data from a "When a card is moved to a specific list" trigger.

## Process Summary
The workflow starts by retrieving the specified list. It then checks the ID of newly moved Trello cards and returns the name and description of the card. A new issue is then created in Linear using the extracted Trello card data, assigning it to a specific project and team. If a name is attached to the card, the issue is also assigned to the corresponding user in Linear.

## Output Details
The workflow creates a new issue in Linear based on the Trello card details, including name, description, project, team, and assigned user.
