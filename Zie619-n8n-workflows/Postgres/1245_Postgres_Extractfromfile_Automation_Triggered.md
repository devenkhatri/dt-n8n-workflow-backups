# Workflow Analysis for Translate questions about e-mails into SQL queries and run them

## Description
This workflow is designed to translate natural language questions about emails into SQL queries and execute them. It integrates multiple services, including database operations and AI-powered query generation, to provide a seamless experience.

## Input Details
The workflow is triggered by a manual trigger or a chat input, and it receives natural language queries as input.

## Process Summary
The workflow first loads the database schema, then uses an AI agent to generate a SQL query based on the natural language input. It checks if the query exists, adds a trailing semicolon if necessary, and executes the query using a Postgres node. The workflow also handles errors, saves files locally, and combines query results with chat answers.

## Output Details
The workflow produces the executed SQL query results, which are then formatted and returned as output.

## Tags
automation, n8n, production-ready, excellent, optimized, sql, postgres, ai, chat
