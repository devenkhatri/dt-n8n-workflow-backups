# Workflow Analysis for Smart Factory Use Case

## Description
This automated workflow processes sensor data from a smart factory, identifies critical temperature conditions, manages incidents, and stores both raw and enriched machine data.

## Input Details
The workflow is triggered by incoming sensor data from factory sensors via an AMQP queue named "berlin_factory_01".

## Process Summary
The workflow receives sensor data, including temperature readings, from an AMQP queue. It checks if the reported temperature is 50°C or higher. If the temperature is high, it creates an incident in PagerDuty and records the incident details in a CrateDB table. Concurrently, it converts the Celsius temperature to Fahrenheit. Finally, it extracts and prepares various sensor and machine metadata, then ingests this comprehensive machine data into a separate CrateDB table.

## Output Details
The workflow either creates an incident in PagerDuty and logs incident information, or it stores processed and enriched machine sensor data in a CrateDB database.

## Tags
smart factory, sensor data, incident management, CrateDB, PagerDuty, temperature monitoring, automation, production-ready, n8n, optimized
