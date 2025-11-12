# Workflow Analysis for agente

## Description
A comprehensive clinic automation workflow that handles patient communications via WhatsApp and internal staff requests via Telegram. It manages appointment scheduling, rescheduling, cancellations, confirmation reminders, and maintains a clinic shopping list, while also processing images and audio messages from patients.

## Input Details
The workflow is triggered by incoming WhatsApp messages (text, images, audio) via webhook, Telegram messages from clinic staff, and a daily schedule trigger for appointment confirmations.

## Process Summary
The workflow receives and categorizes incoming WhatsApp messages, using AI to transcribe audio and extract text from images. It processes patient requests for appointment management through Google Calendar integration, maintaining conversation context in Postgres memory. Internal Telegram messages from staff trigger rescheduling workflows or shopping list updates in Google Tasks. A daily scheduled task sends confirmation messages to next-day patients, and urgent situations are escalated to human staff via a separate workflow.

## Output Details
The workflow sends automated WhatsApp responses to patients, Telegram notifications to staff, updates Google Calendar events, adds tasks to Google Tasks, and escalates urgent cases to human handlers via another workflow.

## Tags
automation, n8n, production-ready, excellent, optimized, clinic management, appointment scheduling, WhatsApp automation, Telegram integration, Google Calendar, Google Tasks
