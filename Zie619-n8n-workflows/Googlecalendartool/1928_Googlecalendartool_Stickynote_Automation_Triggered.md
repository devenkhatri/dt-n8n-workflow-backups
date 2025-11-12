# Workflow Analysis for Reservation Medcin

## Description
This workflow automates appointment scheduling for Dr. Hakim by interacting with patients via chat, checking real-time availability in Google Calendar, booking confirmed appointments, and logging patient details in Google Sheets.

## Input Details
The workflow is triggered manually or potentially by an incoming chat message (though the chat trigger node is currently a placeholder), and receives patient requests including name, phone number, and desired appointment time.

## Process Summary
The AI assistant, powered by OpenAI's GPT-4o-mini, engages with the patient to collect required details (name, phone, desired time). It checks availability in Google Calendar based on office hours and existing bookings. If the requested slot is available, it asks for patient confirmation. Upon confirmation, it creates a calendar event and logs the appointment details in a Google Sheet. The workflow uses memory to maintain conversation context across interactions.

## Output Details
The workflow creates a calendar event in Google Calendar and appends a new row with patient information to a Google Sheet upon successful appointment booking.

## Tags
appointment scheduling, AI assistant, Google Calendar, Google Sheets, healthcare automation, OpenAI, n8n, production-ready
