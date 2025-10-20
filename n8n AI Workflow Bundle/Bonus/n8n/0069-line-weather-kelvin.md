# Workflow Analysis for LINE Weather Kelvin Notification

## Description
This workflow fetches weather data for a specified city in Kelvin and sends a notification via LINE.

## Input Details
This workflow is manually triggered.

## Process Summary
The workflow starts by getting weather data for a specific city from the OpenWeatherMap API. It then converts the temperature from Kelvin to Celsius and finally sends a message with the city name and temperature in Celsius to a LINE Notify group.

## Output Details
The workflow sends a weather notification to a LINE Notify group.
