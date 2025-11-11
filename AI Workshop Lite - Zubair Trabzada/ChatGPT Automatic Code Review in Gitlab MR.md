# Workflow Analysis for GitLab Merge Request Code Review Bot

## Description
This workflow automatically reviews code changes in GitLab merge requests using an AI model and posts structured feedback as a discussion comment on the merge request.

## Input Details
The workflow is triggered by a GitLab webhook when a comment containing '+0' is posted on a merge request.

## Process Summary
When triggered, the workflow fetches the changes in the merge request from GitLab's API and splits them into individual file changes. It filters out renamed or deleted files and ignores diffs that don't start with '@@'. For each relevant code diff, it parses the last affected line numbers, separates original and new code blocks, and sends them to an OpenAI-powered LLM with a prompt to review the code. The LLM's response—structured as a reject/accept decision, score, and suggestions—is posted back to GitLab as a discussion comment on the specific file and line.

## Output Details
The workflow posts AI-generated code review comments directly to the GitLab merge request discussion thread, anchored to the relevant file and line numbers.

## Tags
gitlab, code review, ai, llm, openai, merge request, automation, webhook
