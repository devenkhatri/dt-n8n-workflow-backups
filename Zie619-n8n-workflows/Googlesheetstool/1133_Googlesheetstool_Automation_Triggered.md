# Workflow Analysis for Customer and Sales Support

## Description
This workflow provides an AI-powered customer support and sales assistant for 'My Apple Case' that helps customers check phone case availability, place orders, and automatically updates inventory in real time.

## Input Details
The workflow is triggered manually or via a chat interface where customers send messages asking about phone case availability or placing orders.

## Process Summary
The workflow starts when a customer sends a message. A support agent powered by OpenAI interprets the message and may call the 'GetStock' tool to fetch available cases for a specified phone model from a Google Sheet. If the customer decides to place an order, the agent collects necessary details and uses the 'Place order' node to log the order in a Google Sheet. After the order is placed, the 'Update Stock' node reduces the available quantity and increases the sold count in the inventory sheet. The system follows strict rules to ensure accurate case selection and inventory updates.

## Output Details
The workflow records customer orders in a Google Sheet and updates inventory levels in real time, providing customers with confirmation messages and current stock information.

## Tags
automation, n8n, production-ready, customer support, sales automation, inventory management, Google Sheets, OpenAI, chatbot
