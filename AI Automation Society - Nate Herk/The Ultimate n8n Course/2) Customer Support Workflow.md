# Workflow Analysis for Customer Support Workflow

## Description
This workflow automatically processes incoming Gmail messages, identifies customer support inquiries using AI, generates friendly and informed email responses using a knowledge base, labels the original email, and sends the reply—all without manual intervention.

## Input Details
The workflow is triggered by new emails received in a Gmail inbox, which are then analyzed for customer support content.

## Process Summary
The workflow begins by polling Gmail for new messages. Each incoming email is passed to a text classifier that determines if it's a customer support request or something else. If it's a support query, an AI agent uses a Pinecone-based knowledge base (powered by OpenAI embeddings and the GPT-4o-mini model) to craft a personalized, friendly response with emojis and a signature. The original email is then labeled for tracking, and the generated response is sent as a reply. Non-support emails are ignored.

## Output Details
The workflow sends an automated, AI-generated reply to customer support emails and labels the original message in Gmail for organizational purposes.

## Tags
customer support, email automation, AI response, Gmail integration, natural language processing, knowledge base, Pinecone, OpenAI, classification
