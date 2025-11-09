# Workflow Analysis for Content - Newsletter Agent

## Description
An automated workflow that creates a complete AI newsletter edition by selecting top stories from ingested content, generating compelling subject lines, writing detailed story sections with proper formatting and links, and producing a final markdown newsletter ready for distribution.

## Input Details
Triggered by a form submission that provides a date and previous newsletter content to avoid story duplication.

## Process Summary
The workflow starts by retrieving markdown and Twitter content from storage for the specified date, filtering out non-relevant files. It then uses AI to select the top 4 stories from the collected content while avoiding duplicates from the previous newsletter. After story selection, it generates a compelling subject line and pre-header text. For each selected story, it retrieves full content and external sources, then uses AI to write formatted newsletter sections following specific style guidelines. It also creates an intro section and a 'Shortlist' of other notable AI stories. Finally, it combines all sections into a complete newsletter.

## Output Details
Produces a complete newsletter in markdown format and uploads it to Slack as a file, along with sharing the final content in the designated channel.

## Tags
newsletter, content creation, AI writing, markdown, Slack integration, content curation, automated publishing
