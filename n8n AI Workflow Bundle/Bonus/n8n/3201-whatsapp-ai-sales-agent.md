# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp concerning a product sale, leveraging AI to answer questions, recommend products, and handle sales inquiries.

## Input Details
This workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow begins by receiving a WhatsApp message. It then processes the message using a large language model (LLM) to understand the user's intent and gather relevant information. Based on the LLM's analysis, it utilizes a product database to fetch product details or answer questions. Finally, it constructs a personalized response and sends it back to the customer via WhatsApp.

## Output Details
The workflow outputs a WhatsApp message containing an AI-generated response, product recommendations, or answers to customer queries.
