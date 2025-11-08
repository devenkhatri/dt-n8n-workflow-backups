# Workflow Analysis for AI-Powered GitLab Merge Request Code Review

## Description
This workflow automates code reviews for GitLab merge requests using an AI. When a merge request event is triggered, the AI analyzes code changes, provides feedback, and posts comments directly to the merge request.

## Input Details
The workflow is triggered by a POST webhook, receiving data from GitLab merge request events.

## Process Summary
The workflow starts by receiving a GitLab merge request webhook event and checks a specific condition to determine if a review is needed. If so, it fetches merge request changes from the GitLab API. For each code change (excluding renames or deletions), it parses the diff to extract original and new code snippets along with line number details. An AI model then reviews the extracted code changes and generates a detailed review comment, including a decision and a score.

## Output Details
The workflow posts the AI's detailed code review comments as discussions directly within the relevant GitLab merge request, pinpointing the exact location of the suggestion.
