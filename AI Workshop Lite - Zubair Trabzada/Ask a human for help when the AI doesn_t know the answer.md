# Workflow Analysis for AI Agent with Human Handoff

## Description
This workflow uses an AI agent to respond to user chat inputs. If the AI cannot confidently answer a question, it escalates the query to a human by checking for the user's email; if an email is present, it messages a customer support channel in Slack and informs the user, otherwise it prompts the user to provide their email address.

## Input Details
This workflow is triggered by a chat input from a user.

## Process Summary
First, a user provides an input to an AI agent via a chat trigger. The AI agent, using GPT-4 and a window buffer memory, attempts to answer the user's question. If the AI agent is not confident in its answer, it calls a custom tool that triggers a sub-workflow. This sub-workflow then checks if the user's input contains an email address. If an email is detected, the query is forwarded to a Slack channel for human support, and the user receives a confirmation message. If no email is found, the workflow responds by prompting the user to provide their email address.

## Output Details
The workflow either returns a chat response asking the user for an email or sends a message to a Slack channel and returns a confirmation message to the user.
