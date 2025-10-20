# Workflow Analysis for Twitter Mention Monitor & Discord Notifier

## Description
This workflow monitors Twitter for mentions of a specified user and sends a Discord notification each time a new mention is found. It helps businesses track their brand mentions on Twitter and react promptly.

## Input Details
The workflow is triggered manually and does not receive any specific input data.

## Process Summary
The workflow starts by retrieving the most recent mention ID from a Google Sheet. It then checks Twitter for new mentions of a specified user since that ID. If new mentions are found, it iterates through them, constructs a Discord message containing details of each tweet, and sends the notification to a designated Discord channel. Finally, it updates the Google Sheet with the ID of the latest processed mention.

## Output Details
The workflow sends notifications of new Twitter mentions to a Discord channel.
