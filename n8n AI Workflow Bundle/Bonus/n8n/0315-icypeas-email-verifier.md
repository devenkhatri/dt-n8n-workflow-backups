# Workflow Analysis for Email Verifier using Icypeas API

## Description
This workflow verifies an email address using the Icypeas API and sends a notification to a specific Telegram chat based on the verification result.

## Input Details
This workflow is triggered manually and requires an email address as input.

## Process Summary
The workflow starts by taking an email address as input. It then calls the Icypeas API to verify the provided email address, checking if it is valid. Based on the API response, it sets a custom message indicating whether the email is valid or invalid. Finally, it sends this message to a designated Telegram chat.

## Output Details
The workflow sends a Telegram message indicating whether the input email address is valid or invalid.
