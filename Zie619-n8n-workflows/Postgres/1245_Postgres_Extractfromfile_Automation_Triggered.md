# Workflow Analysis for Translate questions about e-mails into SQL queries and run them

## Description
This workflow translates natural language questions about emails into SQL queries, runs them, and returns the results. It uses various nodes such as Postgres, AI Agent, and Merge to achieve this functionality.

## Input Details
The workflow receives natural language queries as input, either through a chat trigger or a manual trigger, which are then used to generate SQL queries.

## Process Summary
The workflow starts by loading the database schema, then it extracts the table names and columns. It uses an AI Agent to generate a SQL query based on the natural language input. The query is then executed on the Postgres database, and the results are formatted and returned. The workflow also includes error handling and security measures.

## Output Details
The workflow produces the results of the SQL query as output, which can be used for further processing or analysis.

## Tags
automation, n8n, production-ready, excellent, optimized, postgres, sql, natural-language-processing, AI, chatbot
