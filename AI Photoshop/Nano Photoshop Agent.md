# Workflow Analysis for Nano Photoshop Agent

## Description
A Telegram-based AI assistant that helps users manage, edit, and generate images using Google Drive storage and external AI image tools. Users can send photos or text commands to perform actions like renaming files, combining images, editing images, or searching stored images.

## Input Details
The workflow is triggered by messages sent to a Telegram bot, which can include either a photo or text command.

## Process Summary
When a message arrives via Telegram, the workflow checks if it contains a photo or text. If it's a photo, the image is downloaded and uploaded to a Google Drive folder, then the file ID is passed to an AI-powered Photoshop agent. If it's text, it's directly sent to the agent. The agent, powered by either GPT-5 Mini or Claude Sonnet 3.5, uses memory of past interactions and has access to tools for renaming files, combining images, editing images, and searching both raw and AI-generated images in Google Drive. Based on the user's request, the agent selects and executes the appropriate tool and sends a response back to the user via Telegram.

## Output Details
The workflow sends a response message back to the user in Telegram, which may include file links, confirmation messages, or AI-generated responses based on the executed actions.

## Tags
Telegram, Google Drive, AI Agent, Image Editing, File Management, Claude, GPT, Workflow Automation
