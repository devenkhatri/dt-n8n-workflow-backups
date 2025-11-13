# Workflow Analysis for Smart Factory Data Generator

## Description
This workflow simulates and generates smart factory sensor data, including machine ID, temperature, uptime, and a timestamp. The generated data is then automatically sent to a message queue.

## Input Details
The workflow is triggered manually, initiating the data generation process on demand.

## Process Summary
1. The workflow begins when it is manually triggered.
2. A 'Set' node then creates a data payload, which includes a fixed machine ID 'n8n_cr8', a randomly generated temperature in Celsius, a randomly generated machine uptime value, and the current timestamp.
3. Finally, this complete data payload is transmitted to an AMQP message broker, targeting the 'berlin_factory_01' queue.

## Output Details
The workflow outputs the simulated smart factory data to an AMQP queue named 'berlin_factory_01'.

## Tags
automation, n8n, production-ready, excellent, optimized
