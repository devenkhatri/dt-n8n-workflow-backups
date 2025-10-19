# Workflow Analysis for Classify Lemlist Replies with OpenAI and Automate Handling

## Description
This workflow classifies replies received from Lemlist campaigns using OpenAI to understand their intent and then automates actions based on that classification, such as updating a Google Sheet, creating tasks in ClickUp, or sending personalized responses.

## Input Details
The workflow is triggered by a webhook from Lemlist, receiving campaign reply data.

## Process Summary
The workflow starts by extracting and formatting the email body from the Lemlist webhook data. It then uses OpenAI to classify the email content, determining if it's a positive reply, a negative reply, or an out-of-office message. Based on the classification, it updates a Google Sheet with the reply details, including the classification. If the reply is positive, it creates a task in ClickUp and sends a personalized positive reply using Gmail. If the reply is an out-of-office message, it reschedules the campaign in Lemlist.

## Output Details
The workflow updates a Google Sheet, creates tasks in ClickUp for positive replies, sends automated Gmail responses, and reschedules campaigns in Lemlist for out-of-office replies.
