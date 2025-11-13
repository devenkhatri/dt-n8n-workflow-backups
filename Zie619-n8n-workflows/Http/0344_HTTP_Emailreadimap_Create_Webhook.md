# Workflow Analysis for Create Nextcloud Deck card from email

## Description
This workflow automatically reads incoming emails and creates a new card in a Nextcloud Deck board using the email's subject and body content.

## Input Details
The workflow is manually triggered and fetches emails from an IMAP mailbox configured with provided credentials.

## Process Summary
The workflow begins by manually triggering an execution. It then connects to an IMAP email account to fetch unread emails. A function node processes each email to strip HTML tags and format the message body as plain text. Finally, it sends a POST request to the Nextcloud Deck API to create a new card with the email subject as the title and the cleaned body as the description.

## Output Details
The workflow creates a new card in a specified Nextcloud Deck board and stack using authenticated HTTP requests.

## Tags
email, nextcloud, deck, automation, imap, card creation, n8n
