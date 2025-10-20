# Workflow Analysis for ISS Satellite Position and Velocity Monitoring

## Description
This workflow tracks the real-time position and velocity of the International Space Station (ISS) and can notify a Telegram chat about its status.

## Input Details
This workflow is manually triggered.

## Process Summary
The workflow starts by fetching the current location and velocity of the ISS from an external API. It then extracts specific data: longitude, latitude, units, and velocity. This information is then formatted into a readable text message. Finally, it sends this message to a specified Telegram chat.

## Output Details
The workflow sends a message containing the ISS's position and velocity to a Telegram chat.
