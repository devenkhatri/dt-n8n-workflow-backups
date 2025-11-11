# Workflow Analysis for Auto categorize wordpress template

## Description
This workflow automatically categorizes WordPress blog posts using AI by analyzing each post's title and assigning it to the most relevant predefined category.

## Input Details
The workflow is triggered manually and fetches all existing WordPress posts from the connected site.

## Process Summary
The workflow starts by retrieving all WordPress posts. For each post, it sends the title to an AI agent powered by OpenAI, which analyzes the title and assigns a single primary category ID based on a predefined list of categories. The AI's output category ID is then used to update the post's category in WordPress.

## Output Details
The workflow updates each WordPress post with its newly assigned category ID based on AI analysis.

## Tags
wordpress, AI, categorization, automation, content organization, OpenAI
