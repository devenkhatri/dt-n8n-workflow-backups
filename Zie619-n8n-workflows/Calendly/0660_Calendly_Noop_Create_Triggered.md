# Workflow Analysis for Klicktipp Workflow

## Description
This workflow automatically syncs Calendly booking and cancellation events with KlickTipp, ensuring that both invitees and their guests are properly added or removed from marketing lists with accurate event details.

## Input Details
The workflow is triggered by Calendly events (either 'invitee.created' or 'invitee.canceled') and receives event payload data including invitee details, guest emails, event times, and booking links.

## Process Summary
When a Calendly event is created or canceled, the workflow first checks whether it’s a booking or cancellation. For bookings, it formats event timestamps and invitee data into KlickTipp-compatible formats, then subscribes the invitee and any guests to a KlickTipp list. For cancellations, it reads previously stored guest emails from the invitee’s KlickTipp record and unsubscribes both the invitee and guests. Special handling ensures that rescheduled events don’t overwrite guest data, and empty guest fields are reset during cancellations.

## Output Details
The workflow updates subscriber records in KlickTipp by either adding new contacts (for bookings) or updating tags/fields (for cancellations), using the KlickTipp API with transformed Calendly event data.

## Tags
Calendly, KlickTipp, booking automation, event synchronization, email marketing, guest management, cancellation handling, data transformation, n8n workflow, production-ready
