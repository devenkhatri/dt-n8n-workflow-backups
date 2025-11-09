# Workflow Analysis for Content - Newsletter Agent

## Description
An automated workflow that generates a complete AI newsletter edition by selecting top stories from markdown and Twitter content, writing compelling sections with proper formatting, creating subject lines, and producing a final markdown file ready for distribution.

## Input Details
The workflow is triggered by a form submission that provides a date and the previous newsletter content to avoid duplication.

## Process Summary
The workflow retrieves markdown and Twitter content from S3 storage for the specified date, filters out non-relevant content, and selects the top four AI stories using an LLM. It then iterates through each selected story, retrieves full content, and writes detailed newsletter sections following specific formatting guidelines. The workflow also generates an engaging subject line and pre-header text, creates an introductory section, and compiles additional top stories for 'The Shortlist' section. Throughout the process, it shares outputs in Slack for human review and approval before finalizing.

## Output Details
The workflow produces a complete newsletter in markdown format and uploads it as a file to a Slack channel for final distribution.

## Tags
newsletter, content creation, AI, automation, Slack, markdown, LLM
