# Workflow Analysis for AI-Powered On-Brand Article Generation for WordPress

## Description
This workflow leverages AI to automate the creation of new blog article drafts that maintain consistency with an existing brand's style and voice. It achieves this by first analyzing previously published content to learn the article structure, writing styles, and brand voice characteristics, and then uses these guidelines to generate new content.

## Input Details
The workflow is manually triggered and initiates by fetching the latest blog posts from a specified blog URL.

## Process Summary
The workflow fetches the 5 latest article URLs from the n8n blog and retrieves their full content. The extracted HTML content is converted to Markdown and combined. Two separate AI models analyze the combined content: one identifies the common article structure and writing styles, and the other extracts specific brand voice characteristics with descriptions and examples. These analyses are merged with a new article instruction provided by the user. A final AI model, acting as a content generation agent, uses all the gathered guidelines and the instruction to write a new article, extracting its title, summary, and body.

## Output Details
The workflow produces a new blog article draft (including title and content) and saves it to a specified WordPress account.
