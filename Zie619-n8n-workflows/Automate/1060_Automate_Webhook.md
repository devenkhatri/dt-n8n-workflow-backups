# Workflow Analysis for POC - Chatbot Order by Sheet Data

## Description
A proof-of-concept chatbot named Pizzaro that helps customers order pizza by interacting with them, fetching product data from a backend sheet, placing orders, and checking order status—all powered by an AI agent and external API calls.

## Input Details
The workflow is triggered when a user sends a message to the chatbot via a public webhook endpoint.

## Process Summary
When a chat message is received, it is passed to an AI agent configured as 'Pizzaro,' a pizza-ordering assistant. Based on the user's request, the agent can fetch product details, place an order, or check order status by calling external HTTP endpoints that presumably interact with a Google Sheet or similar data source. The workflow includes memory to maintain conversation context and robust error handling for each tool. The entire interaction is designed to simulate a real-world chatbot ordering system.

## Output Details
The workflow returns AI-generated responses to the user via the chat interface, including menu details, order confirmations, or status updates based on data retrieved from or sent to external services.

## Tags
chatbot, pizza order, AI agent, OpenAI, Google Sheets integration, webhook, automation, n8n, production-ready
