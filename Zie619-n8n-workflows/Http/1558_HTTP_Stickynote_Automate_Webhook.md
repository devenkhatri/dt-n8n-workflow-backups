# Workflow Analysis for ✨📊Multi-AI Agent Chatbot for Postgres/Supabase DB and QuickCharts + Tool Router

## Description
Automated workflow: ✨📊Multi-AI Agent Chatbot for Postgres/Supabase DB and QuickCharts + Tool Router. This workflow integrates 13 different services: postgresTool, stickyNote, httpRequest, agent, outputParserStructured. It contains 45 nodes and follows best practices for error handling and security.

## Input Details
The workflow is triggered by an incoming chat message or executed as a sub-workflow, receiving a user prompt, routing information, and potentially database records.

## Process Summary
The workflow begins with a chat message or an external trigger, where a primary AI agent routes the request for either database querying or chart generation. If a database query is needed, a secondary Postgres agent uses an LLM to generate and execute SQL queries against a Postgres database, leveraging schema and table definitions. For chart generation, a secondary QuickChart agent generates a Chart.js configuration based on user prompts and database records. This configuration is then used to construct a QuickChart URL. Throughout the process, chat history is maintained in a Postgres database.

## Output Details
The workflow produces either the results of a SQL query from the Postgres database or a URL for a generated QuickChart, and maintains chat memory.

## Tags
automation, n8n, production-ready, excellent, optimized, AI, chatbot, Postgres, Supabase, QuickCharts, database, charting
