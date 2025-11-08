# Workflow Analysis for Google Analytics: Weekly Report

## Description
This workflow automatically generates a weekly report of Google Analytics data, comparing the last 7 days with the same period of the previous year. It summarizes key metrics, analyzes the performance using AI, and then distributes the report via email and an optional Telegram message.

## Input Details
The workflow is triggered automatically every Monday at 7 AM by a schedule.

## Process Summary
The workflow initiates weekly to retrieve Google Analytics metrics for the past 7 days and the equivalent period of the previous year for a specific property. It then assigns and summarizes the fetched data for both periods. An AI subsequently processes this summarized data to create a comparative table and a concise analysis, formatted for both email and Telegram. Finally, a separate AI model processes the email content to convert it into a suitable plain text format for Telegram.

## Output Details
The workflow sends a comprehensive Google Analytics report as an HTML email and a summarized version as a plain text message to a specified Telegram chat.
