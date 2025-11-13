# Workflow Analysis for Mattermost Webhook

## Description
This workflow receives a webhook from Mattermost, fetches a random drink recipe from an external API, and posts the drink suggestion with instructions and an image back to the originating Mattermost channel.

## Input Details
The workflow is triggered by a POST webhook from Mattermost containing the channel ID in the request body.

## Process Summary
The workflow starts when a POST request is sent to the webhook endpoint. It then makes an HTTP GET request to a configured external API (via BASE_URL environment variable) to fetch a random drink recipe. Using the received drink data, it constructs a formatted message including the drink name, instructions, and serving glass. Finally, it sends this message along with an image attachment back to the Mattermost channel specified in the original webhook payload.

## Output Details
The workflow sends a formatted drink suggestion message with instructions and an image to a Mattermost channel using the Mattermost API.

## Tags
Mattermost, webhook, drink recipe, HTTP request, messaging, automation
