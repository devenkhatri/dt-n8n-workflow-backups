# Workflow Analysis for Daily AI News Translation & Summary with GPT-4 and Telegram Delivery

## Description
This workflow automatically fetches the latest AI-related news from two sources (NewsAPI and GNews), uses GPT-4.1 to select the top 15 articles, translates them into Traditional Chinese while preserving technical English terms, and delivers the formatted summary directly to a Telegram chat every morning at 8am.

## Input Details
The workflow is triggered automatically every day at 8am and fetches news articles from NewsAPI and GNews APIs based on the keyword 'AI'.

## Process Summary
First, the workflow triggers at 8am daily. It then fetches AI-related English news articles from both GNews and NewsAPI. The results from both sources are standardized and merged into a single list. This combined list is sent to GPT-4.1 with a custom prompt instructing it to select the 15 most relevant articles, translate them into Traditional Chinese (keeping technical terms in English), and format them with today’s date and article URLs. Finally, the generated summary is sent to a specified Telegram chat.

## Output Details
The workflow outputs a formatted daily AI news summary in Traditional Chinese and sends it to a configured Telegram chat using a Telegram bot.

## Tags
AI news, translation, GPT-4, Telegram, automation, news aggregation, daily digest, n8n
