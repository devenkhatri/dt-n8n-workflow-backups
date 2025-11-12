# Workflow Analysis for Googlesheets Workflow

## Description
This workflow manages a user waitlist by collecting registration details through a form, generating and emailing a verification code, validating the code through a loop until correct, and finally gathering additional information about the user's intended useâ€”all while storing and updating data in a Google Sheet.

## Input Details
The workflow is triggered by a user submitting a waitlist registration form containing their first name, last name, email, and company website.

## Process Summary
First, the user's input is cleaned and standardized, and a random 6-character verification code is generated. The user's data along with the code is saved to a Google Sheet, and a verification email is sent. The user is then prompted to enter the code via a form; if incorrect, they are asked to re-enter it until valid. Once verified, the user is marked as verified in the sheet and prompted for additional information about their intended use, which is also saved to the same Google Sheet.

## Output Details
The workflow updates a Google Sheet with user data, verification status, and intended use, and sends a verification email to the user.

## Tags
waitlist, google sheets, email verification, form automation, user onboarding, verification code, n8n
