# Workflow Analysis for Discord AI Bot for Feedback Categorization

## Description
This workflow uses an AI model to analyze user feedback received via a webhook, categorizes it, and then routes the categorized feedback with specific instructions to the appropriate department's Discord channel (User Success, IT, or Helpdesk) for further action.

## Input Details
The workflow is triggered by a POST request to a webhook, receiving user feedback in the request body.

## Process Summary
The workflow receives user feedback via a webhook. An OpenAI node analyzes the feedback, categorizing it as a "success-story", "urgent-issue", or "ticket" and generates a concise instruction for the relevant department. A subsequent node parses this JSON response. A switch node then directs the categorized feedback and instruction to one of three different Discord channels based on its category: User Success Department, IT Department, or Helpdesk.

## Output Details
The workflow outputs a message containing the categorized feedback and instructions to a designated Discord channel for either the User Success Department, IT Department, or Helpdesk.
