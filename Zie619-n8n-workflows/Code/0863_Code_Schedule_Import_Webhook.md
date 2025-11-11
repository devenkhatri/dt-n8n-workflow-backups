# Workflow Analysis for Scheduletrigger Workflow

## Description
This workflow automatically fetches today's top Product Hunt posts, resolves their actual website URLs by handling redirects, and saves the product details (name, tagline, description, and clean URL) to a Google Sheet every day.

## Input Details
The workflow is triggered daily by a schedule trigger and uses the current date to fetch Product Hunt posts for that day.

## Process Summary
The workflow starts with a daily schedule trigger that sets today’s date. It then calls the Product Hunt GraphQL API to get the latest posts for that day. The response is parsed to extract product info like name, tagline, description, and website. For each product, it makes an HTTP request to resolve the actual destination URL by capturing the redirect location. It then merges the product information with the resolved URLs, cleans any Product Hunt referral parameters, and appends or updates the combined data in a Google Sheet.

## Output Details
The workflow outputs structured product data into a Google Sheet, including name, tagline, description, and cleaned website URL.

## Tags
automation, Product Hunt, Google Sheets, API integration, scheduled workflow, URL redirection, n8n
