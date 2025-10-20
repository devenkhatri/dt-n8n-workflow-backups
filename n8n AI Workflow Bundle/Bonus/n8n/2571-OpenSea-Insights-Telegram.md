# Workflow Analysis for OpenSea NFT Insights to Telegram

## Description
This workflow monitors new listings and sales on OpenSea for a specified collection and sends real-time notifications to a Telegram chat.

## Input Details
The workflow is triggered manually.

## Process Summary
The workflow starts by retrieving the project slug for a given collection from OpenSea. It then fetches new listings and sales events from OpenSea using the retrieved slug. The workflow processes the event data, formatting it into a human-readable message. Finally, it sends these messages as notifications to a specified Telegram chat.

## Output Details
The workflow sends formatted messages containing OpenSea listing and sales insights to a Telegram chat.
