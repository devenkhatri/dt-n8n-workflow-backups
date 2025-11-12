# Workflow Analysis for Cheems - Scheduled Discord Messages Workflow

## Description
This workflow automatically sends fun and scheduled messages to a Discord channel at specific times of the week and every 30 minutes.

## Input Details
The workflow is triggered automatically by three cron schedules: every Friday at 9 AM, every Saturday at 9 AM, and every 30 minutes.

## Process Summary
The workflow contains three independent cron triggers. One runs every Friday at 9 AM and sends a 'Friday' message to Discord. Another runs every Saturday at 9 AM and sends a 'Wednesday, my dudes!' meme message. The third triggers every 30 minutes and sends a bedtime message. Each message includes a webhook URL from environment variables. An error handler is included to catch and report any execution failures.

## Output Details
The workflow sends scheduled text messages to a Discord channel using a webhook URL defined in environment variables.

## Tags
automation, discord, cron, scheduled messages, n8n, production-ready
