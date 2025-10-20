# Workflow Analysis for Webflow CMS Item to Notion Database Item

## Description
This workflow transfers content from a new or updated Webflow CMS item to a Notion database item.

## Input Details
The workflow is triggered by a Webflow webhook whenever a new item is created or an existing item is updated in a specified CMS collection.

## Process Summary
First, the workflow identifies if the Webflow item was created or updated. If it's a new item, it creates a new page in a Notion database using the Webflow item's data. If the item was updated, the workflow searches for an existing Notion page with a matching Webflow Item ID. If found, it updates that Notion page with the new Webflow data; otherwise, it creates a new Notion page. Finally, it constructs a URL for the updated Notion page if the Webflow item was updated.

## Output Details
The workflow creates a new or updates an existing page in a Notion database.
