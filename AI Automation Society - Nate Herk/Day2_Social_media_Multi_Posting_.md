# Workflow Analysis for AI-Powered Multi-Platform Social Media Post Adaptation

## Description
This workflow automates the process of adapting a single social media post for multiple platforms (LinkedIn, Twitter/X, and Facebook) using AI, then saves the adapted content and previews to a Google Sheet.

## Input Details
The workflow is triggered manually and receives a pre-defined social media post and a topic from a Code node for processing.

## Process Summary
The workflow begins by defining an original social media post and its topic. It then leverages separate AI models to adapt this content for LinkedIn, Twitter/X, and Facebook, adhering to each platform's specific formatting and content guidelines. Subsequently, individual Code nodes refine the AI-generated content, adding appropriate hashtags and creating platform-specific previews. All the formatted posts and their respective previews are then consolidated. Finally, the original post, along with its adapted versions for each platform and a "Ready to Post" status, are appended as a new row to a Google Sheet.

## Output Details
The workflow produces platform-specific adapted social media posts for LinkedIn, Twitter/X, and Facebook, which are then saved, along with the original post and a "Ready to Post" status, into a Google Sheet.
