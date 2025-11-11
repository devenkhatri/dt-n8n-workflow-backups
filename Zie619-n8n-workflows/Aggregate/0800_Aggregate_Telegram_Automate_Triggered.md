# Workflow Analysis for Chinese Vocabulary Learning Bot via Telegram

## Description
This workflow creates an interactive Chinese vocabulary tutor that engages Telegram users with multiple-choice questions based on a Google Sheet vocabulary list, evaluates their answers, and provides immediate feedback—all while maintaining individual conversation memory per user.

## Input Details
The workflow is triggered by a message sent to a Telegram bot and receives the user's chat ID, message text, and first name, along with vocabulary data from a Google Sheet.

## Process Summary
The workflow starts when a user sends a message to a Telegram bot. It retrieves a vocabulary list from a Google Sheet and aggregates Chinese and English words into structured lists. An AI agent, powered by OpenAI's GPT-4o-mini, uses this vocabulary and the user's input to generate multiple-choice questions in Chinese. The AI evaluates the user's response (A, B, C, or D), provides feedback, and automatically generates a new question. All interactions are tied to the user’s Telegram chat ID for personalized conversation memory.

## Output Details
The workflow sends personalized multiple-choice questions and feedback messages back to the user via Telegram.

## Tags
Telegram bot, language learning, Chinese vocabulary, AI tutor, OpenAI, Google Sheets, MCQ generator, conversational AI, educational automation
