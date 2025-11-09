# Workflow Analysis for Content - Newsletter Agent

## Description
An automated workflow that creates a complete AI newsletter by selecting top stories from provided content, generating compelling subject lines, writing detailed story sections with proper formatting and links, and compiling everything into a final markdown document ready for distribution.

## Input Details
The workflow is triggered by a form submission that provides a date and previous newsletter content to avoid duplicates.

## Process Summary
The workflow retrieves markdown and Twitter content from S3 storage for the specified date, filters out irrelevant files, and selects the top four AI stories while excluding previously covered topics. It then generates a compelling subject line and pre-header text, writes detailed newsletter sections for each story following specific formatting guidelines, creates an introduction section, and compiles a 'Shortlist' of other noteworthy AI stories. Throughout the process, it validates external links, extracts relevant images, and shares drafts in Slack for human review and approval before finalizing.

## Output Details
The workflow produces a complete newsletter in markdown format, saves it as a file, uploads it to Slack, and shares a link to the final document.

## Tags
newsletter, content creation, AI, automation, Slack, markdown, Claude, Gemini, S3, content aggregation
