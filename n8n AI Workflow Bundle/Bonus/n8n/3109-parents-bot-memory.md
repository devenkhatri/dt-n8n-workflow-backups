# Workflow Analysis for Parents Bot Memory

## Description
This workflow helps a parent bot remember conversation context by storing and retrieving messages from a Google Sheet, enabling more coherent and personalized interactions.

## Input Details
This workflow is triggered manually and receives no specific input data.

## Process Summary
The workflow starts by clearing old messages from a Google Sheet if the "CLEAR_MEMORY" option is set to true. It then filters messages to keep only the most recent ones based on a specified limit, extracts the last message from the processed data, and converts the remaining messages into a specific JSON format suitable for Google Sheet insertion. Finally, it appends the formatted messages to the Google Sheet and provides the last message to the next step.

## Output Details
The workflow updates a Google Sheet with conversation memory and outputs the last message processed.
