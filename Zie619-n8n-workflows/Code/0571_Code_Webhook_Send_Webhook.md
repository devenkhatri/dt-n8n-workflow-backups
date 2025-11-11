# Workflow Analysis for Daily Order Summary Email Workflow

## Description
This workflow automatically collects incoming orders via a webhook, stores them in Airtable with a timestamp, and sends a daily summary email at 7 PM containing a table of all orders received that day.

## Input Details
The workflow receives individual order data via POST requests to a webhook endpoint containing 'orderID' and 'orderPrice', and is also triggered daily at 7 PM by a schedule.

## Process Summary
When a new order arrives via the webhook, the workflow formats the data with a current timestamp and stores it in an Airtable 'orders' table. Separately, every day at 7 PM, the workflow calculates the time range for the past 24 hours, retrieves all orders from Airtable within that window, converts the results into an HTML table, and emails it as a daily summary.

## Output Details
The workflow produces a daily HTML-formatted email summarizing all orders from the past 24 hours and sends it to a specified Gmail address.

## Tags
order management, daily summary, email automation, Airtable integration, webhook, scheduled workflow, e-commerce
