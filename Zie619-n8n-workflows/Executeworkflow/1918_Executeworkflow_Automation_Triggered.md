# Workflow Analysis for Format US Phone Number

## Description
This workflow cleans and standardizes US phone numbers by extracting digits, validating length and country code, and formatting the number into multiple standardized formats including E.164, national, and international styles.

## Input Details
The workflow is triggered by another workflow and receives a 'Phone Number' input which can be in any common US phone number format (with or without country code, various separators, or extensions).

## Process Summary
First, the workflow strips all non-digit characters from the input phone number. It then checks the length of the digit-only number to determine its validity: numbers with 10 digits are assumed to be US numbers without a country code, those with 11 digits are checked to ensure they start with '1' (the US country code), and others are either corrected or marked invalid. Valid numbers are formatted into multiple standard representations (E.164, national, international, etc.), while invalid numbers are cleared. If a number has more than 11 digits, the extra digits are treated as an extension.

## Output Details
The workflow outputs a structured set of formatted phone number fields including raw input, cleaned number, E.164 format, national format, full national format, international format, and extension (both numeric and string).

## Tags
phone number formatting, US phone number, data cleaning, n8n workflow, E.164 formatting, automation, production-ready
