# Workflow Analysis for SEO Blog Generator with GPT-4o, Perplexity, and Telegram Integration

## Description
This workflow automatically generates SEO-optimized blog posts on men's health topics by combining user-provided research queries with AI-powered content creation and real-time research from Perplexity. It produces a complete blog draft along with a title, URL slug, and meta description, and can deliver the final output directly to a Telegram chat.

## Input Details
The workflow is triggered either by a form submission containing a research query or by a message sent to a Telegram bot.

## Process Summary
First, the workflow accepts a research query via a web form or Telegram message. It then uses an AI agent to refine the query and sends it to a Perplexity-powered research sub-workflow to gather up-to-date information. Using this research, a GPT-4o model generates a full 1500–2000 word SEO-optimized blog post. Separately, another GPT-4o instance creates a title, URL slug, and meta description based on the generated content. Finally, all components are merged and sent back to the user via Telegram.

## Output Details
The workflow sends a complete blog post package—including title, subtitle, content, and hashtags—directly to the Telegram chat where the original request was made.

## Tags
SEO, blog generator, GPT-4o, Perplexity, Telegram, content automation, men's health, AI writing, workflow automation, n8n
