# Workflow Analysis for Code Review workflow

## Description
This workflow automatically reviews GitHub pull requests using AI. When a new pull request is opened, it fetches the code changes, formats them into a structured prompt, and sends them to an AI model (like GPT-4) for review. The AI’s feedback is then posted as a comment on the pull request, and the PR is labeled to indicate it has been reviewed by AI.

## Input Details
The workflow is triggered by a GitHub pull request event and receives the PR metadata and changes via a GitHub webhook.

## Process Summary
1. A GitHub pull request triggers the workflow. 2. The workflow fetches the list of changed files and their diffs using the GitHub API. 3. A code node formats these diffs into a clear, contextual prompt for an AI reviewer, specifying that it should act as a senior iOS developer. 4. The prompt is sent to an AI model (e.g., GPT-4o-mini), optionally enriched with coding best practices from a Google Sheet. 5. The AI’s review is posted as a comment on the original pull request, and a 'ReviewedByAI' label is added to the PR.

## Output Details
The workflow posts an AI-generated code review as a comment on the GitHub pull request and adds a 'ReviewedByAI' label to the PR.

## Tags
github, code review, ai, automation, pull request, gpt, openai, ios, google sheets, n8n
