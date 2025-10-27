# Workflow Analysis for TradingView Chart Analysis with OpenAI

## Description
This workflow analyzes TradingView.com charts using a Chrome extension, n8n, and OpenAI to provide insights and market analysis.

## Input Details
The workflow is manually triggered and uses an HTTP request to receive image data from a Chrome extension. 

## Process Summary
The workflow starts by receiving an image from a Chrome extension via an HTTP request. It then encodes this image data into a Base64 string. The encoded image is sent to OpenAI along with a prompt to analyze the TradingView chart. Finally, the response from OpenAI is extracted and prepared for output.

## Output Details
The workflow outputs a JSON object containing the analysis of the TradingView chart provided by OpenAI.
