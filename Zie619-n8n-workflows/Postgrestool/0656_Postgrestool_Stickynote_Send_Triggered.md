# Workflow Analysis for Stickynote Workflow

## Description
This workflow integrates OpenAI with a Supabase database, enabling users to interact with their data via an AI agent. It dynamically generates SQL queries based on user requests, streamlining data retrieval and analysis.

## Input Details
The workflow is triggered manually and receives data from a chat message.

## Process Summary
The workflow uses an AI agent to analyze user requests and generate custom SQL queries to retrieve data from a Supabase database. It also includes error handling and security measures. The workflow consists of several nodes, including a manual trigger, sticky notes, a chat trigger, an OpenAI chat model, a database schema tool, and a postgres tool. The workflow executes a query to get a list of all tables in the database, and then executes another query to get the definition of a specific table. The workflow also includes a node to run a custom SQL query using knowledge about the output structure to provide the needed response for the user request.

## Output Details
The workflow produces a response to the user based on the data retrieved from the database.

## Tags
automation, n8n, production-ready, excellent, optimized, database, AI, chatbot, Supabase, PostgreSQL, SQL
