# Workflow Analysis for Extract Spending History from Gmail to Google Sheet

## Description
This workflow extracts spending information from your Gmail account and organizes it into a Google Sheet for easy tracking and analysis.

## Input Details
This workflow is triggered every 5 minutes by a Cron node and does not receive any direct input data.

## Process Summary
The workflow starts by fetching emails from Gmail that match specific criteria (from "AMZ Payments" and containing "Your payment of"). It then extracts various details like merchant, date, and amount from each email using regular expressions and string manipulation. Next, it structures the extracted data into a JSON format. Finally, it checks if a Google Sheet exists, and if not, it creates one before appending the processed spending data as new rows.

## Output Details
The workflow outputs structured spending data as new rows in a specified Google Sheet.
