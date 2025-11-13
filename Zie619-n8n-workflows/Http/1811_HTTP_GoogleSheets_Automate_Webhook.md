# Workflow Analysis for Line_Chatbot_Extract_Text_from_Pay_Slip_with_Gemini

## Description
This workflow serves as a Line chatbot that uses Google Gemini AI to intelligently respond to user messages. It can handle both text-based queries and extract structured information from uploaded pay slip images.

## Input Details
The workflow is triggered by incoming messages to a Line Messaging API webhook, receiving either text or image data from a user.

## Process Summary
The workflow starts by receiving a Line message and classifying it as either a text or image type. For text messages, a Google Gemini AI assistant processes the query and generates a response. For image messages, the workflow first retrieves the image content and then utilizes Google Gemini to analyze the image, specifically extracting key details such as Status, From, To, Date, and Amount from a pay slip. Finally, the extracted pay slip data is appended to a Google Sheet.

## Output Details
The workflow sends a text response back to the Line user, which is either a generated text response or the extracted pay slip information, and also records the pay slip data in a Google Sheet.

## Tags
automation, n8n, production-ready, excellent, optimized
