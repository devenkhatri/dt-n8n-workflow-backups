# Workflow Analysis for Klicktipp Workflow

## Description
This workflow automatically captures new form submissions from Gravity Forms, processes the data (like formatting phone numbers, converting dates to timestamps, and scaling ratings), and then subscribes the contact to a KlickTipp mailing list. It also dynamically manages tags by checking if they exist in KlickTipp, creating them if needed, and applying them to the contact for segmentation and automation purposes.

## Input Details
The workflow is triggered by a webhook that receives POST data from Gravity Forms when a new form is submitted.

## Process Summary
The workflow starts by receiving form data via a Gravity Forms webhook. It then formats key fields like phone number, birthday, webinar date, and rating. The formatted data is used to subscribe the contact to a specific KlickTipp list. Separately, the workflow extracts tags from the form response, compares them with existing KlickTipp tags, and either applies existing tags or creates new ones before tagging the contact accordingly.

## Output Details
The workflow subscribes the contact to a KlickTipp list and applies relevant tags (either existing or newly created) to enable targeted email campaigns and automations.

## Tags
gravityforms, klicktipp, contact subscription, tag management, data transformation, webhook automation, email marketing, form automation
