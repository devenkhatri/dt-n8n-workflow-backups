# Workflow Analysis for LinkedIn Content Creator

## Description
This workflow automatically generates engaging LinkedIn posts for entrepreneurs by researching a given topic online and synthesizing insights from multiple articles into a concise, original post with hashtags and emojis.

## Input Details
The workflow is manually triggered and fetches a topic marked as 'To Do' from a specific Google Sheet.

## Process Summary
The workflow starts by retrieving a topic from a Google Sheet where the status is 'To Do'. It then uses the Tavily API to search the web for recent articles related to that topic. The retrieved article content is passed to an AI language model (Claude via OpenRouter) with detailed instructions to create a short, inspiring LinkedIn post. The AI synthesizes the key insights from the articles into an original post under 700 characters, including relevant hashtags and emojis. Finally, the generated content is written back to the Google Sheet, updating the row with the new post and changing the status to 'Created'.

## Output Details
The workflow outputs a ready-to-publish LinkedIn post, which is saved back to the original Google Sheet alongside the topic and with its status updated to 'Created'.

## Tags
linkedin, content creation, AI writing, google sheets, tavily, openrouter, social media automation
