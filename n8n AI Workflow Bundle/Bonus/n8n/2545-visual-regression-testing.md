# Workflow Analysis for Visual Regression Testing with n8n

## Description
This workflow automates visual regression testing for web pages by comparing screenshots and reporting differences.

## Input Details
This workflow is manually triggered.

## Process Summary
The workflow starts by navigating to a specified URL and taking a full-page screenshot as the "new" image. Then, it retrieves an existing "old" image from a specified folder. Both images are compared pixel-by-pixel, and any differences are highlighted and saved as a "diff" image. If differences are found, a notification is sent to a specified chat application (e.g., Mattermost) along with the old, new, and diff images. Finally, the "new" image replaces the "old" image for future comparisons, ensuring continuous monitoring.

## Output Details
The workflow sends a message with comparison results and images to a Mattermost channel and updates a screenshot file on Google Drive.
