# Workflow Analysis for Telegram AI Document Assistant

## Description
This workflow serves as an AI document assistant that processes PDF files received via Telegram, extracts text, answers questions using AI, and responds to the user.

## Input Details
The workflow is triggered by an incoming message to a Telegram bot.

## Process Summary
The workflow receives messages from Telegram and checks for PDF documents. If a PDF is found, it downloads the file, extracts the text content, and saves it in a database. If the message is a question, it retrieves relevant document chunks from the database, sends them to an AI model along with the question, and then sends the AI-generated answer back to the user via Telegram.

## Output Details
The workflow sends AI-generated answers or confirmation messages back to the user via Telegram.
