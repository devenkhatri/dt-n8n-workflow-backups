# Workflow Analysis for Congratulations Workflow

## Description
This workflow automates the process of sending personalized congratulatory SMS messages to individuals for events scheduled on a Google Sheet. It ensures that the right message is sent at the right time based on predefined calendar and message templates.

## Input Details
The workflow is triggered daily at 8 AM by a scheduled cron job and fetches event data from a Google Sheet.

## Process Summary
First, the workflow checks a "Congratulations Calendar" Google Sheet for any events scheduled for the current date. If an event is found, it then retrieves personalized "Congratulations Messages" from another Google Sheet. The event details are merged with the messages based on the event name. Next, a custom function personalizes the congratulatory message using the recipient's first name and extracts their phone number. Finally, the personalized message is sent as an SMS to the corresponding phone number using Twilio.

## Output Details
The workflow sends personalized congratulatory SMS messages to individuals via Twilio.

## Tags
automation,google sheets,twilio,sms,daily trigger,personalized messages,event reminders
