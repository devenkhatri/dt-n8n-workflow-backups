# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow automatically generates and sends personalized voice reminder emails for upcoming real estate appointments by pulling calendar events, creating a tailored voice message using AI, converting it to an audio file, and emailing it to the attendee.

## Input Details
The workflow is triggered manually or on a schedule, and it fetches upcoming calendar appointments from a Google Calendar for the next two days.

## Process Summary
The workflow starts by retrieving upcoming appointments from Google Calendar. For each appointment, it uses an OpenAI language model to generate a personalized voice script and a short email subject based on appointment details like name, time, and location. The script is sent to ElevenLabs API to generate an MP3 voice message. The filename of the MP3 is updated using the email subject, and the file is attached to an email sent via Gmail to the attendee.

## Output Details
The workflow produces an MP3 voice reminder attached to a personalized email sent to the appointment attendee via Gmail.

## Tags
automation, voice reminder, real estate, Google Calendar, OpenAI, ElevenLabs, Gmail, n8n, production-ready
