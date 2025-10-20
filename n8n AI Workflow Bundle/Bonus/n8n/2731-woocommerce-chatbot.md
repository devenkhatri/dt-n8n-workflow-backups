# Workflow Analysis for WooCommerce Chatbot for Product Information

## Description
This workflow automates responding to customer queries about WooCommerce products using AI. When a customer asks a question, the AI chatbot retrieves relevant product information from your store and provides a helpful answer.

## Input Details
This workflow is triggered by an incoming webhook containing a customer question and conversation history.

## Process Summary
The workflow starts by receiving a customer's question and conversation history. It then retrieves product information from WooCommerce based on the customer's query. The product data and conversation history are sent to a large language model (LLM) to generate an AI-powered response. Finally, a custom JavaScript code formats the response, extracting a summary and suggested follow-up questions, which are then used to send a formatted message back to the customer.

## Output Details
The workflow sends a formatted AI-generated response, including a summary and suggested questions, back to the customer via the initial webhook.
