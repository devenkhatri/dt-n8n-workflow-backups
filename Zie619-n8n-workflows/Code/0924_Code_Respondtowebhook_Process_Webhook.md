# Workflow Analysis for WhatsApp Flows Encrypted Data Processor

## Description
This workflow securely processes encrypted data from WhatsApp Flows, decrypts it using RSA and AES encryption, determines the user's current screen context, and returns dynamically encrypted response data for appointment scheduling or seat selection.

## Input Details
The workflow is triggered by an HTTP POST webhook containing encrypted WhatsApp Flow data including encrypted_flow_data, encrypted_aes_key, and initial_vector.

## Process Summary
The workflow receives encrypted WhatsApp Flow data via a webhook, converts the base64-encoded components to buffers, and decrypts them using a private RSA key to extract an AES key, which is then used to decrypt the actual payload. It parses the decrypted JSON to identify the current screen context (like 'APPOINTMENT' or 'DATE_SELECTION_SCREEN'). Based on this, it routes the data through different processing paths: one extracts and groups appointment times by date, while another extracts available seat information. Finally, it constructs a response, encrypts it using AES-GCM with an inverted initialization vector, and returns the encrypted response as base64 text.

## Output Details
The workflow returns an encrypted, base64-encoded JSON response containing either available appointment times with dates or seat selection options, sent back through the original webhook connection to WhatsApp Flows.

## Tags
WhatsApp Flows, encryption, decryption, RSA, AES, webhook, appointment scheduling, seat selection, data processing, secure messaging
