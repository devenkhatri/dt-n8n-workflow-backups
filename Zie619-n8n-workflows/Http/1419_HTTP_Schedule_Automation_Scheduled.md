# Workflow Analysis for Scans von PDF zu Nextcloud

## Description
This workflow automates the process of copying scanned PDF documents to Nextcloud, requiring a USB scanner and a program like ScanServJS with an API.

## Input Details
This workflow is triggered hourly by a schedule and fetches scan data, likely PDF documents, via HTTP requests from a scanning service API.

## Process Summary
First, the workflow is initiated hourly by a schedule trigger. It then performs an HTTP request to an API to retrieve information about scanned documents. Following this, it makes another HTTP request to obtain the actual binary data of the PDF scan. Finally, the workflow uploads these acquired PDF documents to a designated "Scans" folder within Nextcloud, using the document name retrieved earlier.

## Output Details
The workflow uploads scanned PDF documents to a specified folder in Nextcloud.

## Tags
automation, n8n, production-ready, excellent, optimized, Nextcloud, PDF, Scanner, Document Management
