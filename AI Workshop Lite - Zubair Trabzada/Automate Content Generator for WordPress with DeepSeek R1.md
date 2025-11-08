# Workflow Analysis for Automate Content Generator for WordPress with DeepSeek R1

## Description
This workflow automates the creation of SEO-friendly content and accompanying cover images for WordPress blogs. It leverages AI models to generate articles and titles from initial ideas and DALL-E to create visuals, streamlining the content publishing process for blog managers.

## Input Details
The workflow is triggered manually and reads content prompts from a Google Sheet.

## Process Summary
First, it retrieves content prompts from a Google Sheet. Then, DeepSeek R1 generates a detailed article and an SEO-friendly title based on each prompt. Subsequently, it creates a draft WordPress post with this generated content and title. Concurrently, DALL-E generates a cover image based on the article's title, which is then uploaded and set as the featured image for the WordPress post. Finally, the Google Sheet is updated with the article's creation date, generated title, and WordPress post ID.

## Output Details
The workflow produces a new draft WordPress post with AI-generated content, an SEO-friendly title, and a DALL-E generated cover image, and updates the source Google Sheet with post details.
