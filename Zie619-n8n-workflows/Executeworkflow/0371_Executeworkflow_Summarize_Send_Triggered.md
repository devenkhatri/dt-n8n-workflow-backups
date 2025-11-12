# Workflow Analysis for Stickynote Workflow

## Description
This workflow enables a chat interface with an OpenAI assistant that can answer questions about fictional countries and their capitals. It also supports listing all known fictional countries or retrieving the capital of a specific one. Additionally, it includes a tool to return the current date and time.

## Input Details
The workflow is triggered either by a chat message sent via a chat interface or by another workflow execution that passes a 'query' parameter.

## Process Summary
When triggered via chat, the workflow interacts with an OpenAI assistant configured with two custom tools: one to retrieve the current date/time, and another to look up capitals of fictional countries. The fictional country tool works in two modes: if the input query is 'list', it returns all known country names; otherwise, it matches the query to a country and returns its capital. The country data is hardcoded in two code nodes, and matching is done using a merge node. Appropriate responses are formatted and returned based on the query type.

## Output Details
The workflow returns either a list of fictional country names or the capital of a specific fictional country (or an error message if not found), and can also return the current timestamp—responses are sent back to the calling chat interface or parent workflow.

## Tags
OpenAI, chat assistant, fictional data, country capitals, workflow tool, sub-workflow, date tool, conditional logic, n8n, automation
