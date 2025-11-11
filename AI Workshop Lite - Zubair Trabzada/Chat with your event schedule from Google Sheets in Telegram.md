# Workflow Analysis for Telegram-bot AI Da Nang

## Description
An AI-powered Telegram bot that helps members of a meetup group in Da Nang with scheduling and answering questions by using data from a Google Sheet.

## Input Details
The workflow is triggered either by messages sent to a Telegram bot or by chat input within the n8n interface for testing.

## Process Summary
The workflow starts by normalizing input from either Telegram or n8n into a common format. It then fetches schedule data from a Google Sheet and converts it into a markdown table to provide context. This data is passed to an AI agent (LLM) with memory support to generate intelligent responses to user queries. The response is formatted and routed based on the input source—either back to Telegram or to the n8n interface. A typing indicator is sent to Telegram users while the AI is processing the response.

## Output Details
The workflow sends the AI-generated response back to the user either in Telegram or within the n8n interface, depending on where the query originated.

## Tags
telegram, ai, google sheets, chatbot, llm, automation, meetup, scheduling
