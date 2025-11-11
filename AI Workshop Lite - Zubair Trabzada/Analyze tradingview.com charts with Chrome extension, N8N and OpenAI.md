# Workflow Analysis for Chrome Extension Backend with AI

## Description
This workflow powers a Chrome extension that sends a chart image to an AI model for technical market analysis and returns a simplified explanation for novice traders.

## Input Details
The workflow is triggered by a POST request to a webhook endpoint containing a base64-encoded image of a stock or cryptocurrency chart.

## Process Summary
The workflow starts by receiving a base64-encoded chart image via a webhook. It then sends this image to OpenAI's GPT-4o-mini model with a prompt instructing it to analyze the chart as a financial expert and explain market direction in simple terms for beginners, including a disclaimer. The AI-generated analysis is extracted from the response. Finally, the plain-text analysis is sent back as the response to the original webhook request.

## Output Details
The workflow returns the AI-generated plain-text market analysis directly to the client that called the webhook (e.g., the Chrome extension).

## Tags
AI, OpenAI, GPT, image analysis, technical analysis, trading, crypto, stock market, Chrome extension, webhook, finance, n8n
