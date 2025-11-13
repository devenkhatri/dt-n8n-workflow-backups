# Workflow Analysis for Automate assigning GitHub issues

## Description
This workflow automatically assigns GitHub issues to users based on specific actions or comments. It streamlines the process of managing issue assignments within a GitHub repository.

## Input Details
The workflow is triggered by new GitHub issues being opened or new comments being created on existing issues in the 'harshil1712/build-discord-bot' repository.

## Process Summary
First, the workflow checks if a new GitHub issue is opened or a new comment is created. If an issue is opened and contains an 'assign me' phrase with no existing assignees, it assigns the issue to the creator. If a comment is created and contains an 'assign me' phrase, it checks if the issue is unassigned. If unassigned, it assigns the issue to the commenter; otherwise, it replies to the comment stating the issue is already assigned.

## Output Details
The workflow updates GitHub issues by assigning them to users and adding comments to issues.

## Tags
GitHub, Issue Automation, Assignment, Workflow, n8n
