# Workflow Analysis for Threat Intelligence Scan for URLs in a Google Sheet

## Description
This workflow automates the process of scanning URLs for potential threats using VirusTotal and URLScan.io, and then updates the scan results in a Google Sheet.

## Input Details
The workflow is manually triggered and processes URLs from a specified Google Sheet.

## Process Summary
The workflow starts by reading URLs from a Google Sheet. For each URL, it first checks if a VirusTotal scan report already exists. If not, it initiates a scan with VirusTotal. Simultaneously, it performs a URLScan.io scan for each URL. Finally, it formats the scan results and updates the corresponding rows in the Google Sheet with the VirusTotal and URLScan.io report links.

## Output Details
The workflow updates the Google Sheet with VirusTotal and URLScan.io report links for each scanned URL.
