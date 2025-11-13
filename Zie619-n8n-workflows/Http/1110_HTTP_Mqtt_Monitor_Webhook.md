# Workflow Analysis for Remote IOT Sensor monitoring via MQTT and InfluxDB

## Description
This workflow automatically collects temperature and humidity data from a remote IoT sensor (DHT22 on an ESP32) via MQTT, formats the data, and stores it in an InfluxDB time-series database for monitoring and analysis.

## Input Details
The workflow is triggered by an MQTT message published to the 'wokwi-weather' topic, containing JSON-formatted temperature and humidity readings from a DHT22 sensor.

## Process Summary
The workflow starts when an MQTT message is received from a remote ESP32 sensor on the 'wokwi-weather' topic. A JavaScript code node parses the JSON payload and validates that both temperature and humidity are present as numbers. It then formats the data into InfluxDB line protocol (e.g., 'wokwi-weather humidity=45,temp=22'). Finally, an HTTP request node sends this formatted payload to an InfluxDB bucket using a secure API token and environment-based URL.

## Output Details
The formatted sensor data is posted to an InfluxDB bucket via HTTP POST request, enabling time-series storage and visualization of environmental conditions.

## Tags
MQTT, InfluxDB, IoT, sensor monitoring, DHT22, ESP32, automation, time-series data, n8n
