# Workflow Analysis for Webflow Live Item Publish

## Description
This workflow listens for new items in a Webflow collection, publishes them, and then stores the live URL in the item.

## Input Details
The workflow is triggered by a Webflow webhook when a new item is created in a specified collection.

## Process Summary
The workflow receives data about a new Webflow item. It retrieves the item from Webflow, then publishes it. After publishing, it constructs the live URL and updates the Webflow item with this URL.

## Output Details
The workflow updates the original Webflow item with its newly published live URL.
