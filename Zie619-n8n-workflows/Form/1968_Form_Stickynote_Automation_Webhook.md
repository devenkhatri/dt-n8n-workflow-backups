# Workflow Analysis for Social Media Publisher

## Description
This workflow allows users to submit a form with a caption, media file (photo or video), social media platform, and account details, then automatically publishes the content to the selected social media platform using the Upload-post.com API.

## Input Details
The workflow is triggered by a form submission that includes the platform (dropdown), account name, caption (textarea), media file upload (JPEG or MP4), and optional Facebook page ID.

## Process Summary
Upon form submission, the workflow checks whether the uploaded file is a photo (JPEG) or video (MP4) using a switch node. It then routes the data to either the 'Post photo' or 'Post video' HTTP request node, which sends the content to the Upload-post.com API with the provided details. After receiving the API response, it evaluates whether the post was successful using a result parser and conditional logic. Finally, it displays a success or error message to the user via a completion form.

## Output Details
The workflow sends media and metadata to the Upload-post.com API for cross-platform publishing and returns a user-facing success or error confirmation message through a form completion screen.

## Tags
social media, automation, content publishing, form submission, photo upload, video upload, API integration, n8n
