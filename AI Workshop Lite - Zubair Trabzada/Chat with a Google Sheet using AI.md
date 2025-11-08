# Workflow Analysis for Chat with Google Sheet

## Description
This workflow enables an AI agent to interact with a Google Sheet, allowing users to query and retrieve specific data from the spreadsheet through a natural language chat interface. It leverages custom tools to efficiently extract column names, specific column values, or entire customer rows without processing the whole sheet.

## Input Details
The workflow is triggered by a user's chat message, which serves as the input query for the AI agent.

## Process Summary
The main workflow receives a chat message and directs it to an AI Agent. The AI Agent, powered by an OpenAI Chat Model, utilizes custom tools to interact with a Google Sheet. These tools trigger a sub-workflow that first sets the target Google Sheet URL and then retrieves its contents. Based on the operation requested by the AI Agent (e.g., list columns, get column values, or get a specific row), the sub-workflow processes the sheet data accordingly. Finally, the sub-workflow prepares the requested data as a JSON string, which the AI Agent then uses to formulate a natural language response to the user.

## Output Details
The workflow outputs a natural language response to the user's chat query, providing specific data extracted from the Google Sheet.
