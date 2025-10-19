# Workflow Analysis for Automated CV Screening with OpenAI

## Description
This workflow automates the screening of CVs submitted via a Google Form, processes them with OpenAI to extract relevant information, and then notifies the hiring team on Slack.

## Input Details
The workflow is triggered by new form submissions to a Google Form.

## Process Summary
First, the workflow extracts the file ID of the submitted CV from the Google Form data. Next, it downloads the CV from Google Drive and converts the PDF content into text. This extracted text is then sent to OpenAI for analysis to identify and structure key applicant details. Finally, the processed information is sent to the hiring team via a Slack message.

## Output Details
The workflow sends a Slack message containing the extracted CV information to a specified channel.
