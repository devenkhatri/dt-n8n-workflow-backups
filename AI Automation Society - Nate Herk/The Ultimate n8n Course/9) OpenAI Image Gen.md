# Workflow Analysis for OpenAI Image Gen LinkedIn Post

## Description
This workflow automatically generates a professional LinkedIn post on a given topic for a specified audience, creates a matching visual using AI image generation, and emails the post and image to the user.

## Input Details
The workflow is triggered by a form submission that includes the user's email address, the desired topic of the LinkedIn post, and the target audience.

## Process Summary
First, the workflow uses the Tavily search API to gather up-to-date information on the specified topic. Then, a GPT-4.1-powered agent crafts a professional LinkedIn post based on the research and target audience. Another AI agent analyzes the post and generates a detailed image prompt. This prompt is sent to OpenAI's image generation API to create a visual. Finally, the generated post and image are emailed to the user.

## Output Details
The workflow sends an email containing the generated LinkedIn post text and the accompanying AI-generated image as an attachment.

## Tags
linkedin, content creation, ai image generation, email automation, social media, openai, tavily, gpt-4
