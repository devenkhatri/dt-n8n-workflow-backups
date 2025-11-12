# Workflow Analysis for Line Save File to Google Drive and Log File's URL

## Description
This workflow automatically receives files sent via LINE Messenger, validates the file type, saves the file to a structured folder in Google Drive (optionally organized by date and/or file type), logs the file details in a Google Sheet, and optionally sends a confirmation or error message back to the LINE user.

## Input Details
The workflow is triggered by a POST request to a LINE webhook endpoint containing a file message from a LINE user.

## Process Summary
The workflow starts by receiving a file message from LINE and fetching configuration settings from a Google Sheet. It then validates whether the file type is allowed based on the configuration. If valid, it determines the correct Google Drive folder path—creating date-based or file-type-based subfolders if needed—and uploads the file. Finally, it logs the file’s name, type, upload date, and URL in a Google Sheet and optionally replies to the user on LINE with the file link or an error message.

## Output Details
The workflow uploads the file to Google Drive, logs file metadata in a Google Sheet, and optionally sends a reply message back to the LINE user with the Google Drive link or an error notification.

## Tags
LINE, Google Drive, Google Sheets, file upload, automation, webhook, file validation, folder organization, logging, messaging
