# Workflow Analysis for Advance Stock Analysis (both Technical and Trends) Using GPT4o Powered AI Agent

## Description
This workflow provides comprehensive weekly stock analysis by combining technical indicators (like RSI, MACD, Bollinger Bands, and support/resistance levels) with news sentiment from financial articles. It uses AI to generate a detailed, professionally written report in Hebrew, formatted as a responsive HTML email, and sends it directly to the user's inbox.

## Input Details
The workflow is triggered by a form submission where the user provides a stock ticker symbol and an email address.

## Process Summary
The workflow first collects the stock ticker and email from a web form. It then fetches and analyzes both technical chart data (using Chart-img, Twelve Data API, and OpenAI vision) and news sentiment (via Alpha Vantage). An AI agent (GPT-4o) synthesizes this data into a structured JSON report with a detailed technical analysis, sentiment summary, top news articles, and a clear investment recommendation, all in Hebrew. This JSON is used to generate a styled HTML email, which is then sent to the user's provided email address.

## Output Details
The workflow produces a detailed stock analysis report in the form of a responsive HTML email in Hebrew and sends it to the user's email address.

## Tags
stock analysis, AI agent, GPT-4o, technical analysis, news sentiment, HTML email, Hebrew, investment, n8n workflow, automated report
