# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp concerning a new AI course by acting as a sales agent. It leverages AI to answer questions, handles payments, and provides course information.

## Input Details
The workflow is triggered by an incoming WhatsApp message containing text content, typically questions from potential customers about the AI course.

## Process Summary
The workflow first extracts the message details and sets up a chat conversation with context from a Google Sheet acting as a knowledge base. It then uses an AI model to generate a response based on the customer's question and the provided context. If the AI response suggests a payment, the workflow checks for payment intent and, if confirmed, generates a Stripe checkout link. Finally, it formats the AI-generated or payment-related response for WhatsApp.

## Output Details
The workflow sends automated messages via WhatsApp back to the customer, providing answers to their questions, course information, or a Stripe checkout link for payment.
