# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow overlays a background image with a top image (such as a logo or watermark), positioning the top image at the center of the background. It’s useful for automatically adding watermarks or branding to images.

## Input Details
The workflow is triggered manually and fetches two images from URLs defined in the WEBHOOK_URL environment variable—one for the background and one for the overlay.

## Process Summary
The workflow starts by manually triggering the execution. It then fetches two images via HTTP requests—one for the background and one for the top overlay. Metadata (like dimensions) is extracted from both images. The binary data of each image is renamed for clarity, and both items are merged into a single data item. Using the image dimensions, the workflow calculates the center point to position the top image over the background. Finally, it composites the two images together with the top image centered on the background.

## Output Details
The workflow produces a single composite JPEG image with the top image overlaid at the center of the background image, stored in the binary property 'bg'.

## Tags
image processing, watermark, overlay, automation, n8n, manual trigger, image composite, production-ready
