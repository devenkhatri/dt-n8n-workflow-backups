# Workflow Analysis for Google Analytics: Weekly Report

## Description
This workflow automatically generates and sends a weekly Google Analytics performance report comparing the last 7 days of data with the same period from the previous year. It includes key metrics like page views, users, sessions, purchases, and revenue, formatted into a professional HTML email and an optional Telegram message.

## Input Details
The workflow is triggered automatically every Monday at 7 AM via a schedule trigger.

## Process Summary
The workflow starts by fetching Google Analytics data for the last 7 days, then assigns and summarizes the metrics. It calculates the corresponding date range for the previous year and retrieves matching historical data, which is also assigned and summarized. An AI model processes both data sets to generate a comparative HTML table with a brief summary for email, and a simplified plain-text version for Telegram. The final report is sent via email and optionally via Telegram message.

## Output Details
The workflow sends a formatted HTML email with the analytics report to a specified email address and optionally sends a condensed version as a Telegram message.

## Tags
google analytics, weekly report, email automation, telegram notification, data comparison, AI analysis, scheduled workflow
