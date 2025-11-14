# Workflow Analysis for Crypto News & Sentiment

## Description
This workflow automates the process of fetching and analyzing cryptocurrency news and sentiment. It takes a user query from Telegram, gathers relevant articles from multiple crypto news RSS feeds, and uses an AI model to summarize the news and determine market sentiment.

## Input Details
The workflow is triggered by a message sent to a Telegram bot, receiving the user's query for crypto or company name analysis.

## Process Summary
A Telegram message containing a crypto or company name triggers the workflow and the chat session ID is stored. An AI agent extracts a single keyword from the user's message. The workflow then fetches the latest articles from nine different cryptocurrency news RSS feeds. All fetched articles are merged and then filtered to include only those relevant to the extracted keyword. A prompt is constructed using the filtered articles and the original user query for an AI model. An OpenAI GPT-4o model processes the prompt to generate a summary of the news and analyze market sentiment.

## Output Details
The workflow sends a comprehensive AI-generated summary, including news, market sentiment, and links to reference articles, back to the user via Telegram.

## Tags
automation, n8n, production-ready, excellent, optimized, crypto, news, sentiment analysis, telegram bot, AI, RSS, market analysis
