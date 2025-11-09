# Workflow Analysis for Tool - Email Research Report

## Description
This workflow takes a research report written in Markdown format along with an email address and subject line, converts the Markdown content into HTML, and sends it as an email using Gmail.

## Input Details
The workflow is triggered manually or via another workflow and receives three inputs: markdown-formatted report content, an email address, and a subject line.

## Process Summary
The workflow starts by receiving Markdown content, an email address, and a subject line. It then converts the Markdown content into HTML format using a built-in Markdown node. Finally, it sends an email via Gmail using the provided email address as the recipient, the given subject line, and the converted HTML content as the email body.

## Output Details
The workflow sends an HTML-formatted email via Gmail to the specified recipient with the research report in the email body.

## Tags
email, markdown, html conversion, gmail, research report, automation
