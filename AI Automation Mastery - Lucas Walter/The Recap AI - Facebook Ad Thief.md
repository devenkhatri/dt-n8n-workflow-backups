# Workflow Analysis for Facebook Ad Thief with AI Recap

## Description
This workflow automates the process of extracting information from Facebook Ad Library, summarizing it using AI, and storing the insights in Google Sheets.

## Input Details
This workflow is manually triggered.

## Process Summary
First, it prompts the user to input a Facebook Ad Library URL, then it scrapes the ad details from the given input. Afterward, it extracts ad details like heading and body, then it uses OpenAI to summarize the ad content. Finally, it stores the original ad details and the AI-generated summary into a Google Sheet.

## Output Details
The workflow outputs a Google Sheet containing the original Facebook ad details (heading and body) and an AI-generated summary of the ad.
