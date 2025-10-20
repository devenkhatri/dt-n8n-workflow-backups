# Workflow Analysis for Bot Handoff to Human Agent

## Description
This workflow manages the intelligent handoff of a customer conversation from a chatbot to a human agent, specifically designed for platforms like Intercom.

## Input Details
This workflow is triggered manually and receives conversation data as input.

## Process Summary
The workflow begins by checking if a bot action should be performed. If a bot action is not required, it identifies the agent to whom the conversation should be assigned. It then sends a message to the agent within the conversation and finally assigns the conversation to the identified agent.

## Output Details
The workflow assigns the conversation to a human agent within Intercom and sends a notification message.
