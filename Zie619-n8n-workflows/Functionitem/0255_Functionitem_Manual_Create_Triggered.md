# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow manually triggers the retrieval of customer data, sorts it by name, generates personalized invoice templates for each customer, and sends individual text emails. It also compiles a list of all customers into a single HTML email summarizing new customers.

## Input Details
The workflow is triggered manually by a user clicking 'execute' and does not receive external input data.

## Process Summary
The workflow starts with a manual trigger, then retrieves all customer records from a datastore. It sorts the customer list alphabetically by name. For each customer, it adds fixed invoice line items and total amounts using a function node. It then generates individual plain-text invoice emails using a document template and sends them. Separately, it creates a single HTML email listing all customers and sends that as well.

## Output Details
The workflow sends two types of emails: individual plain-text invoice emails per customer and one combined HTML email listing all customers, both sent to a predefined recipient.

## Tags
manual trigger, customer data, email automation, invoice generation, document template, sorting, n8n, production-ready
