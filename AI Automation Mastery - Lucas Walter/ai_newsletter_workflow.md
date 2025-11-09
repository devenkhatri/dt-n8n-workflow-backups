# Workflow Analysis for Content - Newsletter Agent

## Description
An automated workflow that generates a complete AI newsletter by selecting top stories from markdown and Twitter content, writing engaging sections with proper formatting and links, creating a compelling subject line, and publishing the final newsletter as a markdown file to Slack.

## Input Details
The workflow is triggered by a form submission that provides a date and previous newsletter content to avoid duplicates.

## Process Summary
The workflow first retrieves markdown and Twitter content from S3 storage for the specified date, filtering out non-markdown files and newsletter content. It then uses AI to select the top four stories, sharing these selections in Slack for human approval with the ability to provide feedback for revisions. After story approval, it generates a compelling subject line and pre-header text, also shared for approval. The workflow then writes detailed newsletter sections for each selected story, including proper markdown formatting, external links, and image extraction. Finally, it composes the complete newsletter with intro, main stories, and 'Shortlist' sections, then uploads the final markdown file to Slack.

## Output Details
The workflow produces a complete newsletter in markdown format and uploads it as a file to a Slack channel, along with sharing messages containing the final content.

## Tags
newsletter, content-generation, AI-writing, slack-integration, markdown, content-curation
