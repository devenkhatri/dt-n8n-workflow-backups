# Workflow Analysis for WhatsApp and KlickTipp Integrated Messaging Workflow

## Description
This workflow automates personalized WhatsApp messaging triggered by KlickTipp subscriber events and processes user replies to either provide support responses or manage message subscriptions. It enables seamless multi-channel communication using pre-approved WhatsApp templates filled with dynamic subscriber data.

## Input Details
The workflow is triggered either by an incoming WhatsApp message or by a KlickTipp outbound event (e.g., when a subscriber is tagged or updated).

## Process Summary
The workflow starts by receiving either a WhatsApp message or a KlickTipp event. If a WhatsApp message is received, it checks whether the message starts with 'STOP' (case-insensitive and space-agnostic). Messages not starting with 'STOP' are ignored, while those that do trigger an auto-responder template and subscribe the user to an opt-out list in KlickTipp. If triggered by KlickTipp, the workflow sends a personalized WhatsApp offer template using subscriber data such as first name, product name, and a custom link. All operations use pre-approved WhatsApp message templates and properly formatted phone numbers.

## Output Details
The workflow sends WhatsApp message templates to users and optionally subscribes their phone numbers to a KlickTipp list for opt-out management.

## Tags
WhatsApp, KlickTipp, marketing automation, message template, subscription management, two-way messaging, n8n
