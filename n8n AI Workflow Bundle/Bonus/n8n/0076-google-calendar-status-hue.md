# Workflow Analysis for Google Calendar Status to Philips Hue Light

## Description
This workflow checks your Google Calendar for ongoing events and updates your Philips Hue smart lights to reflect your calendar status (busy or available). This is useful for indicating to others whether you are in a meeting or free.

## Input Details
This workflow is triggered every minute by a Cron node.

## Process Summary
The workflow starts by getting the upcoming calendar events from Google Calendar. It then checks if there are any events currently happening. Based on the event status, it sets a variable to "busy" or "available". Finally, it controls Philips Hue lights, turning them red if busy and green if available, using a custom scene.

## Output Details
The workflow controls Philips Hue smart lights, setting their color to red (busy) or green (available) based on Google Calendar events.
