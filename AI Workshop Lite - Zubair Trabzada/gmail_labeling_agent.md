# Workflow Analysis for Gmail Labeling Agent with AI

## Description
This workflow automates the categorization and labeling of incoming Gmail messages using artificial intelligence.

## Input Details
The workflow is triggered manually and does not receive any specific input data.

## Process Summary
The workflow starts by retrieving unread emails from a specified Gmail account. Then, for each email, it extracts the email body to determine if the message is a "newsletter." Next, based on the email content, it classifies the email into one of four categories: "Marketing," "Social," "Promotions," or "Forums" using a text classification model. Finally, the workflow applies the relevant labels to the email in Gmail, marks it as read, and moves it to the appropriate category.

## Output Details
The workflow updates Gmail by applying labels, marking emails as read, and moving them to categorized folders.
