# Workflow Analysis for Technical Analyst Agent vs. Workflow

## Description
This workflow provides automated technical analysis of stock charts using AI. It accepts a stock ticker and exchange, generates a chart with technical indicators like MACD and volume, analyzes the chart using GPT-4o, and sends both the chart image and detailed analysis via Telegram.

## Input Details
The workflow is triggered either by another workflow (providing ticker and exchange) or by a Telegram message (user query about a stock).

## Process Summary
The system first obtains the stock ticker and exchange, either directly from a workflow trigger or by parsing a user’s Telegram message using AI. It then requests a technical chart from the chart-img API with MACD and volume indicators. The generated chart image is downloaded and analyzed by GPT-4o using a detailed prompt for technical financial analysis. Finally, both the chart image and the AI-generated analysis are sent back to the user via Telegram.

## Output Details
The workflow outputs a technical analysis of a stock chart and the chart image itself, both delivered to the user through Telegram messages.

## Tags
stock analysis, technical analysis, AI agent, Telegram bot, GPT-4o, financial chart, MACD, volume analysis, workflow automation
