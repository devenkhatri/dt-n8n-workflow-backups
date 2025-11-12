# Workflow Analysis for CSRD XHTML Report Auditor

## Description
This workflow automatically audits incoming CSRD XHTML sustainability reports by checking for required disclosures and formatting issues, then sends a summary email with findings to the sender.

## Input Details
The workflow is triggered by a new email in Gmail with 'CSRD Reporting' in the subject line and an attached XHTML report.

## Process Summary
The workflow first checks if the incoming email subject contains 'CSRD Reporting'. If so, it downloads the email attachment, extracts the XHTML content, and runs a series of validation checks including presence of header, governance and strategy tags, KPI disclosures, empty tags, and duplicate content. The audit results are then passed to an AI agent that generates a professional summary email. Finally, the workflow replies to the original sender with the audit summary.

## Output Details
The workflow sends a reply email to the original sender with a human-readable summary of the CSRD report audit findings.

## Tags
CSRD, ESG, sustainability, compliance, audit, XHTML, email automation, AI, n8n, reporting
