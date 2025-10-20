# Workflow Analysis for Automated Website Visual Regression Testing

## Description
This workflow automates visual regression testing for websites by comparing current website screenshots against baseline images to detect any visual changes. It provides a robust way to monitor website aesthetics and functionality.

## Input Details
This workflow is triggered manually and requires the URL of the website to be tested.

## Process Summary
The workflow starts manually and receives a website URL. It then takes a full-page screenshot of the provided URL and resizes the image to a standardized width. A comparison is made between the newly captured screenshot and a baseline image. Based on the comparison, it determines if there are visual differences, and if so, it sends an email notification with the comparison results.

## Output Details
The workflow sends an email notification with a visual comparison report (including before/after images and a diff image) if visual differences are detected between the current and baseline website states.
