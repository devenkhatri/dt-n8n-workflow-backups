# Workflow Analysis for HITL Example Flows

## Description
This workflow demonstrates two human-in-the-loop (HITL) approaches for AI-generated social media posts. It automatically creates X (Twitter) posts based on user requests via Telegram, uses web search to gather current information, and then either requests simple yes/no approval or allows detailed feedback for revisions before publishing.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, containing requests to create social media posts.

## Process Summary
The workflow starts by receiving a post request via Telegram. It uses an AI agent with web search capabilities (Tavily) to generate a factual, engaging X post. In the first flow, it sends the post for simple yes/no approval via Telegram before publishing or sending a denial message. In the second flow, it requests open-ended feedback, classifies the feedback as approved or needing revisions, and either publishes the post or uses another AI agent to revise it based on the feedback before republishing.

## Output Details
The workflow either publishes a post to X (Twitter), sends a denial message back to Telegram, or iteratively revises and publishes the post based on human feedback.

## Tags
human-in-the-loop, telegram, x, twitter, social media, ai agent, approval workflow, content creation, tavily, openrouter
