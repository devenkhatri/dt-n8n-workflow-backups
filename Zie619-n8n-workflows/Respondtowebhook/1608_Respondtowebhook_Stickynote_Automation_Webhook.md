# Workflow Analysis for Chrome Extension Backend with AI

## Description
This workflow serves as a backend for a Chrome extension, leveraging Artificial Intelligence to perform financial chart analysis.

## Input Details
The workflow is triggered by an incoming POST request to a webhook, expecting a base64 encoded image of a stock or cryptocurrency chart.

## Process Summary
1. The workflow starts by receiving a financial chart image via a webhook from a Chrome extension.
2. This image is then sent to an OpenAI model configured as an expert financial analyst.
3. The AI analyzes the provided chart using various technical indicators to predict market movements and generates simplified insights for novice traders.
4. Finally, the AI-generated financial analysis, along with a disclaimer, is returned as a text response to the Chrome extension.

## Output Details
The workflow produces a text-based financial analysis from the OpenAI model, which is sent back as the response to the initial webhook call.

## Tags
automation, n8n, production-ready, excellent, optimized
