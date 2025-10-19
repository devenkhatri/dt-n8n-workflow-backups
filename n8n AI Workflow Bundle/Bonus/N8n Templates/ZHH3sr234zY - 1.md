# Workflow Analysis for AI Lead Classification and Sales Routing with Conditional Forwarding

## Description
This workflow automatically receives new data, such as a contact form submission or a chat message, via a webhook, uses an AI model (GPT-3.5-turbo) to classify the incoming text into categories like 'Sale Lead', 'Support Request', 'General Inquiry', 'Feedback', or 'Other'. Based on the classification, it conditionally routes 'Sale Lead' items to an external automation platform (Make/Integromat) for specialized processing, and then sends a final response back to the original webhook caller.

## Input Details
The workflow is triggered by an incoming HTTP request (Webhook) which is expected to contain a text query (`$json.query`) that needs to be classified.

## Process Summary
The workflow starts with a Webhook trigger that receives incoming data, including the text to be analyzed. Next, the 'AI Classify Lead' node uses GPT-3.5-turbo to categorize the text into one of five predefined types: 'Sale Lead', 'Support Request', 'General Inquiry', 'Feedback', or 'Other'. The 'Set Category' node extracts the classification result from the AI node and attaches it to the workflow data. An IF node ('Is Sales Lead?') checks if the classification is 'Sale Lead'. If the condition is true, the data is forwarded to an external system (Make/Integromat) via an HTTP Request for further sales handling; finally, the 'Respond to Webhook' node sends a completion status back to the original caller.

## Output Details
The workflow returns an immediate HTTP response (status 200) to the original Webhook caller, confirming that the process has finished and including the final classified category.
