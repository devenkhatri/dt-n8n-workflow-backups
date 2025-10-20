# Workflow Analysis for AI WordPress Article Creator

## Description
This workflow automates the creation and publishing of WordPress articles using AI, triggered by a new row in a Google Sheet which contains article specifications like keyword, focus keyword, image style, etc. It generates images, titles, content, and metadata, then publishes the article to WordPress.

## Input Details
The workflow is triggered by new rows added to a specified Google Sheet, providing article details such as the primary keyword, focus keyword, desired image style, and other relevant information.

## Process Summary
The workflow starts by retrieving new article data from a Google Sheet. It then generates image prompts based on the article details using AI and creates an image. Next, it uses AI to generate a compelling article title, slug, and meta description. Subsequently, it generates the main article content using AI. Finally, it constructs the full article with the generated images and text, and publishes it to WordPress, including setting the feature image.

## Output Details
The workflow publishes a complete, AI-generated article, including images and metadata, directly to a specified WordPress site.
