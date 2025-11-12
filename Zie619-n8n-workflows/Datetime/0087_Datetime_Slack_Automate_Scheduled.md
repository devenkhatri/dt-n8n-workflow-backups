# Workflow Analysis for Weekly Shopify Order Summary Report

## Description
This workflow automatically retrieves Shopify orders once a week, calculates the total number of orders and their combined value, and shares the summary in a Slack channel while also logging the data in a Google Sheet.

## Input Details
The workflow is triggered weekly at 10 AM UTC by a cron scheduler and fetches order data from Shopify.

## Process Summary
The workflow starts by fetching all orders from Shopify. It then processes each order’s creation date and filters out orders before a specific date (August 17, 2021). For qualifying orders, it extracts and retains only the total price as 'orderPrice'. A function node aggregates these orders to compute the total count and sum of order values. Finally, the results are sent to a Slack channel and appended to a Google Sheet.

## Output Details
The workflow outputs a summary message to a Slack channel and appends the aggregated order data to a specified Google Sheet.

## Tags
Shopify, Slack, Google Sheets, reporting, automation, cron, weekly report, order summary
