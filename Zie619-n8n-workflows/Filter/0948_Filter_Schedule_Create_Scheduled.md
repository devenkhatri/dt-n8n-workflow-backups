# Workflow Analysis for Daily Customer Churn Win-Back Offer Automation

## Description
This workflow automatically identifies customers at high risk of churn each day and sends them personalized win-back offers via email based on their predicted churn score and preferred product categories.

## Input Details
The workflow is triggered daily by a schedule and fetches customer data from a Google Sheet containing fields like customer ID, email, predicted churn score, and preferred categories.

## Process Summary
The workflow starts by fetching customer data from a Google Sheet. It then filters customers with a predicted churn score greater than 0.7. If eligible customers are found, it processes each one individually: using Google Gemini to generate a personalized win-back offer (informational message, bonus points, or discount) based on their churn score and preferred categories. The offer details are logged in a system log sheet, and the offer is sent via Gmail. If no eligible customers are found, a 'NOT_FOUND' status is logged instead.

## Output Details
The workflow logs all actions (either sent offers or 'NOT_FOUND' status) in a SYSTEM_LOG Google Sheet and sends personalized win-back emails to eligible customers via Gmail.

## Tags
churn prevention, customer retention, email automation, Google Sheets, Gmail, AI offer generation, scheduled workflow, n8n
