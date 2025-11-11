# Workflow Analysis for Notion to Webflow Blog Post Sync

## Description
This workflow automatically syncs blog posts from Notion to Webflow. It checks for posts marked for syncing, converts Notion content into rich HTML, ensures slugs are unique, and either creates new Webflow posts or updates existing ones based on matching slugs. A success message is sent to Slack upon completion.

## Input Details
The workflow is triggered on a schedule and pulls all blog posts from a specified Notion database, filtering only those with the 'Sync to Webflow?' checkbox enabled.

## Process Summary
The workflow first retrieves all Notion blog posts and filters those marked for syncing. It ensures each post has a unique slug, then fetches full page data including cover images and content blocks. The content blocks are converted into HTML-rich text suitable for Webflow. The workflow then compares Notion slugs with existing Webflow posts to decide whether to create a new post or update an existing one. Finally, it updates Notion with the Webflow item ID and slug, and sends a success notification to Slack.

## Output Details
The workflow creates or updates blog posts in a Webflow collection, updates the corresponding Notion page with the Webflow item ID and slug, and sends a success message to a Slack channel.

## Tags
Notion, Webflow, blog sync, rich text conversion, scheduled automation, CMS integration, Slack notification
