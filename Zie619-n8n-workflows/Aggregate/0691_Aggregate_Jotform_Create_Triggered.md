# Workflow Analysis for Klicktipp Workflow

## Description
This workflow automatically processes new webinar registrations submitted via JotForm, formats the data appropriately, adds the contact to KlickTipp as a subscriber, and applies dynamic tags based on the user’s webinar selection, date, and reminder preferences.

## Input Details
The workflow is triggered by a new form submission from JotForm containing webinar registration details such as name, email, phone number, LinkedIn URL, work experience, birthday, selected webinar, date/time, and reminder preferences.

## Process Summary
When a new JotForm submission arrives, the workflow first reformats and validates the data—converting phone numbers to international format, dates to UNIX timestamps, validating URLs, and scaling numerical values. It then adds the contact to a KlickTipp subscriber list with mapped custom fields. Simultaneously, it extracts dynamic tags from the form (e.g., webinar name, date, reminder interval), checks if those tags already exist in KlickTipp, and either applies existing tags or creates new ones before tagging the contact. The workflow includes robust error handling and uses aggregation and merging logic to manage tag assignment efficiently.

## Output Details
The workflow adds the registrant as a subscriber in KlickTipp with properly formatted contact details and applies relevant tags for segmentation and automation purposes.

## Tags
JotForm, KlickTipp, webinar registration, contact sync, tag automation, data transformation, lead management, subscriber management
