# Workflow Analysis for Klicktipp Workflow

## Description
This workflow automatically syncs Calendly booking and cancellation events with KlickTipp, ensuring that both invitees and their guests are added or removed from KlickTipp subscriber lists with all relevant event details. It handles time zone conversions, guest list management, and distinguishes between cancellations and rescheduling to maintain accurate contact data.

## Input Details
The workflow is triggered by Calendly events (either 'invitee.created' or 'invitee.canceled') and receives event data including invitee details, guest emails, event times, time zone, and rescheduling/cancellation flags.

## Process Summary
First, the workflow receives a Calendly event and determines if it's a booking or cancellation. For bookings, it formats event and invitee data into KlickTipp-compatible formats (e.g., Unix timestamps, seconds since midnight), extracts guest emails, and subscribes both the invitee and guests to a KlickTipp list with relevant event metadata. For cancellations, it checks if guests were part of the original booking by reading stored guest emails from the invitee's KlickTipp record, then unsubscribes both invitee and guests using a cancellation tag. The workflow also handles rescheduling by preserving guest email data and avoids overwriting it in such cases.

## Output Details
The workflow updates subscriber records in KlickTipp by either adding new subscribers (for bookings) or re-tagging existing ones (for cancellations), ensuring accurate contact segmentation based on booking status.

## Tags
Calendly, KlickTipp, booking automation, event management, guest handling, cancellation handling, rescheduling, email marketing, subscriber sync, time zone conversion
