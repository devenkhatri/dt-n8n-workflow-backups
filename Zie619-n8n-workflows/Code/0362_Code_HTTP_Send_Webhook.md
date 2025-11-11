# Workflow Analysis for xSend and check TTS (Text-to-speech) voice calls end email verification

## Description
This workflow provides a dual-factor verification system by sending a voice call with a spoken verification code via text-to-speech (TTS) and a separate verification code via email. Users submit a form with their phone number, email, preferred voice, and language. The system then places a call with the spoken code and emails another code. Verification is completed only when both codes are correctly entered by the user.

## Input Details
The workflow is triggered by a user submitting a form containing their phone number, email address, preferred voice (male/female), language, and name.

## Process Summary
Upon form submission, the workflow assigns a fixed 5-digit verification code for the voice call and another for the email. The voice code is formatted with spaces between digits for clearer TTS pronunciation. A voice call is initiated via the ClickSend API using the provided phone number, selected voice, and language. Simultaneously, an email with the email verification code is sent via SMTP. The user is then prompted to enter both codes through separate verification forms. The workflow checks if both codes match the expected values and displays either a success message or an error if either code is incorrect.

## Output Details
The workflow concludes by showing the user a success message if both verification codes are correct, or an error message if either code is invalid, displayed via completion forms in the browser.

## Tags
voice verification, email verification, TTS, two-factor authentication, ClickSend, form automation, n8n, production-ready
