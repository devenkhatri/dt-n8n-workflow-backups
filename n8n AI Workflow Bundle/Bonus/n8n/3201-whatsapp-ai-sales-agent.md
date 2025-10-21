# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI to answer questions, recommend products, and even process orders through a payment link.

## Input Details
The workflow is triggered by an incoming message to a WhatsApp business account.

## Process Summary
Upon receiving a WhatsApp message, the workflow checks if it's the first interaction. It then uses an AI model (ChatGPT) to understand the user's query and generate a relevant response, including product recommendations or payment links if an order is being placed. If the user expresses product interest, the workflow retrieves product details from a database and presents them. If the user confirms a purchase, the workflow generates a payment link and sends it to the user.

## Output Details
The workflow sends automated, AI-generated responses and payment links back to the customer on WhatsApp.
