# Workflow Analysis for Material Inventory Management with Google Sheets and Telegram

## Description
This workflow automates the management of material inventory by interacting with Google Sheets and sending notifications via Telegram. It allows for adding, updating, and querying material data, ensuring real-time inventory tracking and communication.

## Input Details
The workflow is triggered manually by an HTTP request that includes parameters for the action to be performed (add, update, get, delete) and relevant material data.

## Process Summary
The workflow begins by receiving an HTTP request and determining the action required using a Switch node. If the action is "add", it processes the input data, formats it for Google Sheets, and appends a new row. If the action is "update", it queries the sheet, finds the matching row, updates the data, and then sends the updated row back to Google Sheets. If the action is "get", it queries the sheet based on a provided ID, retrieves the material data, and formats it for output. For each action, it constructs a confirmation message and sends it via Telegram, then returns an HTTP response.

## Output Details
The workflow sends notifications to a specified Telegram chat and returns an HTTP response indicating the success or failure of the operation, along with relevant data.
