# Workflow Analysis for GitLab MR Auto-Review & Risk Assessment

## Description
This workflow automatically reviews GitLab merge requests (MRs) using AI to assess code changes for risk, generate actionable recommendations, identify potential issues, and create test cases for QA. It then posts a detailed review as a comment on the MR and emails a formatted report to relevant developers, QA testers, and global stakeholders.

## Input Details
The workflow is triggered by GitLab webhook events when a merge request is created or updated, receiving MR metadata and associated code diffs.

## Process Summary
First, the workflow captures MR details from a GitLab webhook and merges the payload. It then fetches the actual code diff via GitLab’s API. If changes are detected, it sends the diff to Anthropic’s Claude AI model to analyze for risks, issues, recommendations, and QA test cases. The AI’s structured output is used to generate a rich HTML comment that is posted back to the GitLab MR. Simultaneously, a distribution list of relevant team members is built based on the project name, and a comprehensive HTML email report is sent to developers, QA, global admins, and the MR author.

## Output Details
The workflow posts an AI-generated review comment on the GitLab merge request and sends a detailed HTML-formatted email report to a dynamically generated list of developers, QA testers, global admins, and the MR author.

## Tags
GitLab, merge request, code review, AI analysis, risk assessment, automated testing, email notification, Claude AI, code quality, DevOps automation
