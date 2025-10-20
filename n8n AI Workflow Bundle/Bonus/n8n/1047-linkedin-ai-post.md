# Workflow Analysis for AI-Powered LinkedIn Post Generator

## Description
Leverage AI to generate engaging LinkedIn posts based on a provided topic and keywords, then publish them automatically.

## Input Details
This workflow is manually triggered and receives a topic and relevant keywords for the LinkedIn post.

## Process Summary
First, the workflow uses a Cohere language model to generate several LinkedIn post ideas based on the input topic and keywords. Then, it uses another Cohere model to rewrite one of the generated ideas in an engaging tone. Finally, it uses a Google Gemini model to suggest relevant hashtags for the post before publishing it to LinkedIn and sending a notification to Discord.

## Output Details
The workflow publishes a generated LinkedIn post with AI-suggested hashtags and sends a Discord notification upon completion.
