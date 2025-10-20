# Workflow Analysis for Customer Support Ticketing System

## Description
This workflow automates the customer support ticketing process by integrating email with a CRM and a notification system.

## Input Details
The workflow is triggered by new incoming emails, checking every minute.

## Process Summary
The workflow starts by reading unread emails from a specified inbox. It then categorizes the emails by training and sending them to an AI model. Based on the classification, it creates a new ticket in the CRM and sends a Slack notification.

## Output Details
The workflow creates a customer support ticket in a CRM and sends a notification to a Slack channel.
