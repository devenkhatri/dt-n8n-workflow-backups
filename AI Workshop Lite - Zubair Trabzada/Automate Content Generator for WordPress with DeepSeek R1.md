# Workflow Analysis for Automate Content Generator for WordPress with DeepSeek R1

## Description
This workflow automatically generates SEO-friendly blog posts using DeepSeek R1 based on prompts from a Google Sheet, creates matching cover images using DALL-E, publishes the content as a draft on WordPress, attaches the image, and updates the Google Sheet with publication details.

## Input Details
The workflow is triggered manually (or can be scheduled) and pulls content prompts from a Google Sheet where only the 'Prompt' column is filled in.

## Process Summary
The workflow starts by reading unparsed content prompts from a Google Sheet. It sends each prompt to DeepSeek R1 to generate a full SEO-optimized article in HTML format. Then, it uses the generated article to create an SEO-friendly title. With the title and content ready, it creates a draft post in WordPress. Simultaneously, it generates a realistic cover image using DALL-E based on the title, uploads the image to WordPress, and links it as the featured image of the post. Finally, the workflow updates the original Google Sheet with the current date, generated title, and WordPress post ID.

## Output Details
The workflow produces a draft blog post on WordPress with a generated SEO-friendly title, HTML-formatted content, and a DALL-E-generated cover image, while also updating the source Google Sheet with metadata like publication date, title, and post ID.

## Tags
wordpress, content-generation, deepseek, dall-e, google-sheets, seo, automation, ai-writing, image-generation
