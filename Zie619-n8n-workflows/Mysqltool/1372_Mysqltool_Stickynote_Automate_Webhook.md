# Workflow Analysis for Modelo do Chatbot

## Description
This workflow automates a chatbot interaction, handling incoming chat messages, processing them with AI, and leveraging various data sources to provide comprehensive responses. It is designed for production use with robust error handling.

## Input Details
This workflow is triggered manually or by chat input, receiving messages and optional lead data containing user information like name, age, location, profession, device, channel, and desired quotation type.

## Process Summary
The workflow first determines if detailed lead data is provided; if so, it constructs a comprehensive user profile message for the chatbot. Otherwise, it uses the direct chat input. This prepared input is then processed by an OpenAI assistant to generate responses, and the entire conversation history is stored in a PostgreSQL database for chat memory. Additionally, the workflow can query a MySQL database for product information based on user criteria, access an external knowledge base via an HTTP request, and interact with an external API to retrieve or verify lead details like name and birthdate.

## Output Details
The workflow produces AI-generated responses from an OpenAI assistant, stores chat history and potentially lead data in a PostgreSQL database, and queries product information from a MySQL database, which would then be used to formulate responses back to the user.

## Tags
automation, n8n, production-ready, excellent, optimized, chatbot, AI, OpenAI, Postgres, MySQL, CRM
