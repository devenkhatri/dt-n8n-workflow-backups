# Workflow Analysis for GitLab Code Review with OpenAI

## Description
This workflow automates the process of generating code reviews for new merge requests in GitLab using OpenAI. It fetches the code changes, sends them to OpenAI for review, and then posts the review comments back to the GitLab merge request.

## Input Details
The workflow is triggered by a webhook from GitLab whenever a new merge request is created or updated in a specified project.

## Process Summary
The workflow starts by retrieving the project ID and merge request ID from the GitLab webhook data. It then uses the GitLab API to fetch the changes made in the merge request. These changes are then formatted and sent to OpenAI for a code review. Finally, the review comments from OpenAI are posted back to the GitLab merge request as a system-generated comment.

## Output Details
The workflow posts the AI-generated code review comments as a system note on the corresponding GitLab merge request.
