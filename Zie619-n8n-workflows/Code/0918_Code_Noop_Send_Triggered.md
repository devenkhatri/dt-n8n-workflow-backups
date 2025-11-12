# Workflow Analysis for Informationextractor Workflow

## Description
This workflow automates the process of extracting structured order information (items, quantities, and table numbers) from natural language messages received via a restaurant chatbot, validates the data, and logs each order item into a Google Sheet with a timestamp.

## Input Details
The workflow is triggered by a chat message containing a customer's order, passed from another workflow ("Restaurant POS workflow") via an executeWorkflowTrigger.

## Process Summary
First, an Information Extractor node attempts to parse the order text to extract items, quantities, and table number using regex patterns. An If node checks if the extraction succeeded (i.e., the extract array is not empty). If data was extracted, a custom Python code node processes the raw extraction results into a structured list of order items. A Loop Over Items node then splits this list so each item can be handled individually. Finally, each item is appended as a new row in a Google Sheet along with a timestamp. If no data was extracted, the workflow ends without logging.

## Output Details
The workflow outputs validated order details (item, quantity, table number, and timestamp) as individual rows in a specified Google Sheet.

## Tags
restaurant, order processing, information extraction, google sheets, chatbot, n8n, automation, data parsing, POS
