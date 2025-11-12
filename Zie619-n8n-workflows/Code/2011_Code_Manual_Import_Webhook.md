# Workflow Analysis for Import multiple Manufacturers from Google Sheets to Shopware 6

## Description
This workflow automates the process of importing manufacturer data—including names, websites, descriptions, and logos—from a Google Sheet into a Shopware 6 store. It supports multilingual translations and ensures manufacturer logos are uploaded and linked correctly.

## Input Details
The workflow is manually triggered and pulls manufacturer data from a predefined Google Sheet that contains columns for name, website, description, logo URL, and optional multilingual fields.

## Process Summary
The workflow begins by setting key configuration values like the Shopware URL and default language. It then fetches manufacturer records from a Google Sheet. For each record, it constructs a formatted import payload with support for multiple language translations and generates a unique media ID for the logo if provided. The workflow imports each manufacturer into Shopware via an API call, and if a logo is specified, it uploads the logo file separately and associates it with the manufacturer. The entire process is handled one manufacturer at a time using a batch loop.

## Output Details
The workflow creates or updates manufacturer entries in Shopware 6 and uploads associated logo files when provided, using authenticated API requests to a configured Shopware instance.

## Tags
Shopware 6, Google Sheets, manufacturer import, e-commerce automation, multilingual support, logo upload, n8n workflow, production-ready
