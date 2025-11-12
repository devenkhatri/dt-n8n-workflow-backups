# Workflow Analysis for Convert image from jpg/png to webp

## Description
This workflow automatically converts JPG or PNG images to the more efficient WEBP format using an external API. It pulls image URLs from a Google Sheet, processes them based on file type, converts them via APYHub, uploads the resulting WEBP files to Google Drive, and updates the original sheet to mark the task as completed.

## Input Details
The workflow is manually triggered and receives image URLs from a specified Google Sheet where each row contains a source image URL in the 'FROM' column.

## Process Summary
The workflow starts by manually triggering and setting an API key. It then fetches rows from a Google Sheet containing image URLs. A code node extracts the filename and file extension from each URL. A switch node routes JPG/JPEG and PNG files to their respective HTTP request nodes that call the APYHub conversion API. The converted image is downloaded as a file, uploaded to a designated Google Drive folder with a .webp extension, and the original sheet is updated with the new WEBP URL and a 'DONE' marker.

## Output Details
The workflow uploads converted WEBP images to Google Drive and updates the source Google Sheet with the new image URLs and completion status.

## Tags
image conversion, webp, jpg to webp, png to webp, google sheets, google drive, APYHub, automation, n8n, production-ready
