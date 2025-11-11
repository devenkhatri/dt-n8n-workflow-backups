# Workflow Analysis for Splitinbatches Workflow

## Description
This workflow automatically creates Linear issues from Notion to-do items. It uses a form to accept a Notion page URL and a Linear team name, then processes unchecked to-do blocks that haven’t already been synced to Linear. For each valid to-do item, it extracts the title and potential assignee, shortens the title if needed, fetches the full block content to build a rich description, creates a new issue in Linear, and updates the original Notion block with a link to the newly created issue.

## Input Details
The workflow is triggered by an n8n form submission that includes a Notion page URL and a Linear team name.

## Process Summary
First, the workflow fetches all blocks from the provided Notion page and filters for unchecked to-do items that don’t already contain a Linear link. It queries Linear to find the team and its members based on the team name provided in the form. For each to-do item, it parses the title and potential assignee from the first line, validates the assignee against the team members, and shortens the title using AI if it's too long. It then retrieves the full nested content of the Notion block, converts it to Markdown, and constructs a detailed issue description. Finally, it creates the issue in Linear, fetches the issue URL, and updates the original Notion to-do block with a link to the Linear issue.

## Output Details
The workflow creates new issues in Linear and updates the corresponding Notion to-do blocks with links to those issues, and returns a success or error message to the form submitter.

## Tags
Notion, Linear, issue tracking, automation, form trigger, AI, markdown, to-do sync, workflow automation, n8n
