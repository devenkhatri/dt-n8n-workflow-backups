# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI to respond to queries, qualify leads, and connect them with sales.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by extracting information from the incoming WhatsApp message. It then sends an API request to an AI model to generate a response based on the customer's query and predefined sales guidelines. The AI's response is then sent back to the customer via WhatsApp. Additionally, if the AI identifies a qualified lead, it can notify a sales team member via Slack.

## Output Details
The workflow sends automated AI-generated responses to WhatsApp users and can optionally send lead notifications to Slack.
