# Workflow Analysis for Chrome Extension Backend with AI for Financial Analysis

## Description
This workflow serves as a backend for a Chrome extension, leveraging AI to perform technical analysis on stock or cryptocurrency charts and provide simplified insights for novice traders.

## Input Details
The workflow is triggered by a POST request to a webhook, which expects an image (likely base64 encoded) of a stock or cryptocurrency chart.

## Process Summary
The workflow begins by receiving an image of a stock or crypto chart via a webhook. This image is then sent to an OpenAI model (gpt-4o-mini), which is configured to act as an expert financial analyst. The AI performs an advanced technical analysis of the chart, generating simple insights and market movement expectations tailored for novice traders, along with a disclaimer. Finally, the AI-generated analysis is returned as a text response to the initial webhook call.

## Output Details
The workflow produces a text response containing the AI-generated financial analysis, which is sent back to the client that initiated the webhook request.
